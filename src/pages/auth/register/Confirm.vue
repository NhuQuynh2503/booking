<script setup lang="ts">
import { confirmEmailApi } from '@/services/auth'
import { useLoadingStore } from '@/stores/loading'
import { useConfirmDialog } from '@/stores/modal'

const loadingStore = useLoadingStore()

const confirmDialog = useConfirmDialog()

import { useI18n } from 'vue-i18n'
const { t } = useI18n()

const router = useRouter()
const route = useRoute()

const confirmEmail = async (token: string) => {
  try {
    await confirmEmailApi(token)
    confirmDialog.setQuestion({
      title: 'Success',
      question: t('question.confirm_account_success'),
      onlyConfirm: true,
      actionConfirm: () => {
        router.push({ name: 'login' })
      },
    })
  } catch (error) {
    confirmDialog.setQuestion({
      title: 'Failed',
      question: t('question.confirm_account_failed'),
      onlyConfirm: true,
      actionConfirm: () => {
        router.push({ name: 'login' })
      },
    })
  }
}

onBeforeMount(async () => {
  const token = route.query.token as string
  loadingStore.setLoading(true)
  if (token) {
    await confirmEmail(token)
    loadingStore.setLoading(false)
  } else {
    router.push({ name: 'login' })
  }
})
</script>
<template><div></div></template>
