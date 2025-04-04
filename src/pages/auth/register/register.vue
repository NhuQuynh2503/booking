<script setup lang="ts">
import { Input } from '@/components/ui/input'
import ErrorMessage from '@/components/base/ErrorMessage.vue'
import { Button } from '@/components/ui/button'

import { useForm } from 'vee-validate'
import * as yup from 'yup'
import { registerApi } from '@/services/auth'
import { apiExceptionHandler } from '@/utils/exceptionHandler'

const { errors, handleSubmit, defineField } = useForm({
  validationSchema: yup.object({
    email: yup.string().email().required('Email is required'),
    name: yup.string().required('name is required'),
    password: yup.string().required('Password is required'),
  }),
})

const [email, emailAttrs] = defineField('email')
const [password, passwordAttrs] = defineField('password')
const [name, nameAttrs] = defineField('name')

const router = useRouter()
const onSubmit = handleSubmit(async (values) => {
  try {
    const data = await registerApi({
      email: values.email,
      name: values.name,
      password: values.password,
    })
    console.log(data)
    router.push({ name: 'login' })
    notify.success('Register success')
  } catch (error) {
    notify.error(apiExceptionHandler(error).message)
  }
})
</script>
<template>
  <div class="h-full flex p-8">
    <div class="flex-1 flex justify-center items-center">
      <form
        class="form-shadow p-6 rounded-xl"
        @submit="onSubmit"
      >
        <div class="flex items-center gap-0.5 mb-4">
          <h1 class="text-[344054] text-lg font-semibold">Register account</h1>
        </div>
        <div>
          <h2 class="mt-1 text-[#667085]">Today is a new day. It's your day. You shape it.</h2>
          <h2 class="mt-1 text-[#667085]">Sign in to start managing your projects</h2>
        </div>
        <div class="mt-6">
          <div class="form-data">
            <Label for="email">Name</Label>
            <Input
              v-model="name"
              placeholder="Enter name..."
              v-bind="nameAttrs"
              :invalid="errors.name"
              type="text"
              class="h-10 mt-1"
            />
            <ErrorMessage :error="errors.name" />
          </div>
          <div class="form-data">
            <Label for="email">Email</Label>
            <Input
              v-model="email"
              placeholder="Enter email..."
              v-bind="emailAttrs"
              :invalid="errors.email"
              type="email"
              class="h-10 mt-1"
            />
            <ErrorMessage :error="errors.email" />
          </div>
          <div class="form-data">
            <Label for="email">Password</Label>
            <Input
              v-model="password"
              placeholder="Enter password..."
              v-bind="passwordAttrs"
              :invalid="errors.password"
              type="password"
              class="h-10 mt-1"
            />
            <ErrorMessage :error="errors.password" />
          </div>
        </div>
        <Button class="mt-6 w-full h-10"> Sign Up </Button>
        <div class="flex items-center gap-2 w-full mt-8">
          <span class="h-px bg-slate-200 w-full"></span>
          <p class="text-base">Or</p>
          <span class="h-px bg-slate-200 w-full"></span>
        </div>
        <Button
          class="h-10 mt-8 w-full flex items-center gap-4 bg-zinc-200"
          variant="secondary"
        >
          <img
            class="w-5"
            src="@/assets/img/google-logo.png"
            alt=""
          />
          Sign in with Google
        </Button>
        <div class="flex justify-center mt-6">
          <p>If you have an account?</p>
          <RouterLink
            class="ml-[6px] text-[#0921D9] font-semibold"
            to="/login"
          >
            Sign in
          </RouterLink>
        </div>
      </form>
    </div>
    <div class="flex-1 relative max-md:hidden">
      <img
        class="absolute top-0 left-0 w-full h-full object-cover rounded-3xl"
        src="@/assets/img/auth-bg.png"
        alt=""
      />
    </div>
  </div>
</template>
<style scoped>
.form-shadow {
  box-shadow:
    0px 1px 3px 0px rgba(16, 24, 40, 0.1),
    0px 1px 2px 0px rgba(16, 24, 40, 0.06);
}
</style>
