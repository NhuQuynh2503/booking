<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-logo">
        <span class="blue">Elite</span><span class="gray">Booking</span>
      </div>

      <nav class="footer-nav">
        <ul>
          <li><a href="#">Trang chủ</a></li>
          <li><a href="#">Khách sạn</a></li>
          <li><a href="#">Phòng</a></li>
          <li><a href="#">Giới thiệu</a></li>
          <li><a href="#">Liên hệ</a></li>
        </ul>
      </nav>

      <div class="social-media">
        <a href="#"><i class="fab fa-facebook"></i></a>
        <a href="#"><i class="fab fa-twitter"></i></a>
        <a href="#"><i class="fab fa-instagram"></i></a>
      </div>
    </div>

    <!-- Copyright -->
    <div class="copyright">
      &copy; 2025 EliteBooking. All rights reserved.
    </div>
  </footer>
</template>

<script setup></script>

<style scoped>
.footer {
  background: #1e3a8a;
  color: white;
  padding: 40px 0;
  text-align: center;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  max-width: 1300px;
  margin: 0 auto;
}

.footer-logo {
  font-size: 28px;
  font-weight: bold;
}

.footer-logo .blue {
  color: white;
}

.footer-logo .gray {
  color: #ddd;
}

.footer-nav ul {
  list-style: none;
  display: flex;
  gap: 30px;
}

.footer-nav ul li a {
  text-decoration: none;
  font-size: 18px;
  color: #ddd;
  transition: color 0.3s;
}

.footer-nav ul li a:hover {
  color: white;
}

.social-media a {
  font-size: 24px;
  color: white;
  margin: 0 10px;
  transition: color 0.3s;
}

.social-media a:hover {
  color: #ddd;
}

.copyright {
  margin-top: 20px;
  font-size: 16px;
  color: #ccc;
}
</style>
