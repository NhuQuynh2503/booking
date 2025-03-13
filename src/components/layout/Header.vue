<template>
  <header class="header">
    <div class="container">
      <div class="logo">
        <span class="blue">Elite</span><span class="gray">Booking</span>
      </div>
      <nav class="nav">
        <ul>
          <li><a href="#" class="active">Trang chủ</a></li>
          <li><a href="#">Khách sạn</a></li>
          <li><a href="#">Phòng</a></li>
          <li><a href="#">Giới thiệu</a></li>
          <li><a href="#">Liên hệ</a></li>
        </ul>
      </nav>
      <button class="login-btn">Đăng nhập</button>
    </div>
  </header>
</template>

<script setup>

</script>

<style scoped>
.header {
  background: white;
  padding: 20px 0; 
  border-bottom: 2px solid #ddd;
}


.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1300px; 
  margin: 0 auto;
  padding: 0 40px;
}

.logo {
  font-size: 32px; 
  font-weight: bold;
}

.logo .blue {
  color: #1E40AF;
}

.logo .gray {
  color: gray;
}

.nav ul {
  list-style: none;
  display: flex;
  gap: 30px;
}

.nav ul li a {
  text-decoration: none;
  font-size: 18px;
  color: #111;
  font-weight: bold;
  transition: color 0.3s;
}

.nav ul li a:hover,
.nav ul li a.active {
  color: #1E40AF;
}

/* Login Button */
.login-btn {
  background: #1E40AF;
  color: white;
  border: none;
  padding: 12px 24px;
  font-size: 18px;
  border-radius: 8px;
  font-weight: bold;
  cursor: pointer;
  transition: background 0.3s, transform 0.2s;
}

.login-btn:hover {
  background: #15317E;
  transform: scale(1.05);
}
</style>
