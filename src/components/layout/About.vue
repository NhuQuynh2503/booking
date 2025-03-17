<script setup lang="ts">
import Header from '@/components/layout/Header.vue'
import Footer from '@/components/layout/Footer.vue'
</script>

<template>
  <Header />

  <main class="about">
    <div class="container">
      <h1>Giới Thiệu Về Chúng Tôi</h1>
      <p>
        Chào mừng bạn đến với <span class="highlight">EliteBooking</span>! Chúng tôi cung cấp dịch vụ đặt phòng khách sạn hàng đầu với 
        trải nghiệm người dùng mượt mà, tiện lợi và nhanh chóng.
      </p>

      <section class="about-content">
        <div class="about-box">
          <div class="icon">🚀</div>
          <h2>Sứ Mệnh</h2>
          <p>Đem đến cho khách hàng dịch vụ đặt phòng tốt nhất với mức giá hợp lý.</p>
        </div>

        <div class="about-box">
          <div class="icon">🌍</div>
          <h2>Tầm Nhìn</h2>
          <p>Trở thành nền tảng đặt phòng hàng đầu tại Việt Nam và khu vực Đông Nam Á.</p>
        </div>

        <div class="about-box">
          <div class="icon">💎</div>
          <h2>Giá Trị Cốt Lõi</h2>
          <ul>
            <li>✔ Chất lượng dịch vụ</li>
            <li>✔ Uy tín và minh bạch</li>
            <li>✔ Hỗ trợ khách hàng tận tâm</li>
          </ul>
        </div>
      </section>

      <!-- Khung mô tả du lịch -->
      <section class="description-box">
        <h2>Kinh nghiệm du lịch Việt Nam</h2>
        <p>
          Việt Nam là một điểm đến hấp dẫn với vẻ đẹp thiên nhiên tuyệt vời, văn hóa phong phú và ẩm thực đa dạng. 
          Từ những bãi biển tuyệt đẹp như Phú Quốc, Nha Trang đến những vùng núi hùng vĩ như Sapa, Mộc Châu, mỗi địa danh 
          đều mang một nét đặc trưng riêng, thu hút hàng triệu du khách mỗi năm.
        </p>
        <p>
          Khi du lịch tại Việt Nam, bạn không thể bỏ lỡ những điểm đến nổi bật như Hà Nội – nơi giao thoa giữa cổ kính và hiện đại, 
          Hội An – thành phố di sản thế giới với những con đường đèn lồng rực rỡ, hay Đà Nẵng – thiên đường du lịch với biển xanh 
          cát trắng. Ngoài ra, những trải nghiệm như thưởng thức ẩm thực đường phố, khám phá các làng nghề truyền thống hay tham gia 
          các lễ hội văn hóa sẽ giúp bạn hiểu thêm về đời sống và con người nơi đây.
        </p>
        <p>
          Hệ thống <strong>EliteBooking</strong> giúp bạn dễ dàng tìm kiếm và đặt phòng tại hàng ngàn khách sạn, nhà nghỉ, homestay trên khắp cả nước. 
          Với giao diện trực quan, tiện lợi và nhiều ưu đãi hấp dẫn, chúng tôi cam kết mang đến trải nghiệm du lịch tuyệt vời nhất cho bạn. 
          Hãy để EliteBooking đồng hành cùng bạn trên mọi hành trình!
        </p>
      </section>
    </div>
  </main>

  <Footer />
</template>

<style scoped>
/* Nền gradient tím xanh */
.about {
  padding-top: 110px;
  text-align: center;
  background: linear-gradient(135deg, #F4F5F7, #DCE3F2);
  padding-bottom: 60px;
}

/* Container */
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Tiêu đề */
h1 {
  font-size: 38px;
  font-weight: bold;
  color: #1D3557;
  margin-bottom: 20px;
  text-transform: uppercase;
}

/* Chữ màu nổi bật */
.highlight {
  color: #E63946;
  font-weight: bold;
}

/* Đoạn mô tả */
p {
  font-size: 18px;
  color: #555;
  line-height: 1.6;
}

/* Bố cục nội dung */
.about-content {
  display: flex;
  gap: 30px;
  justify-content: center;
  margin-top: 40px;
}

/* Box từng mục */
.about-box {
  flex: 1;
  background: white;
  padding: 30px;
  border-radius: 15px;
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s, box-shadow 0.3s;
  text-align: center;
  position: relative;
}

/* Hiệu ứng hover */
.about-box:hover {
  transform: translateY(-10px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
}

/* Icon */
.icon {
  font-size: 42px;
  margin-bottom: 10px;
  color: #E63946;
}

/* Tiêu đề trong box */
.about-box h2 {
  font-size: 22px;
  color: #1D3557;
  margin-bottom: 10px;
  font-weight: bold;
}

/* Danh sách giá trị cốt lõi */
.about-box ul {
  list-style: none;
  padding: 0;
}

.about-box ul li {
  font-size: 18px;
  color: #444;
  margin: 8px 0;
  font-weight: 500;
}

/* Khung mô tả du lịch */
.description-box {
  margin-top: 50px;
  padding: 30px;
  border: 2px solid #1D3557; /* Viền màu xanh đậm */
  border-radius: 10px;
  background: #fff;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
  text-align: left;
}

.description-box h2 {
  font-size: 26px;
  color: #1D3557;
  margin-bottom: 15px;
}

.description-box p {
  font-size: 18px;
  color: #333;
  line-height: 1.6;
}
</style>
