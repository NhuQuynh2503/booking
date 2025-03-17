<template>
  <div>
    <div class="hero">
      <h1>Tìm & đặt phòng khách sạn với <br />các bước đơn giản!</h1>
      <p>Khám phá ngay những ưu đãi tốt nhất dành cho bạn tại <b>Booking</b>!</p>
    </div>
    <div class="search-box">
      <div class="input-group">
        <label>Địa điểm tên khách sạn</label>
        <input type="text" placeholder="Nhập địa điểm hoặc tên khách sạn" />
      </div>
      <div class="input-group">
        <label>Ngày nhận phòng</label>
        <input type="date" />
      </div>
      <div class="input-group">
        <label>Ngày trả phòng</label>
        <input type="date" />
      </div>
      <div class="input-group">
        <label>Số lượng</label>
        <input type="number" min="1" value="1" />
      </div>
      <button class="search-btn">Tìm kiếm</button>
    </div>
    <!-- Điểm đến nổi bật
    <div class="destination-section">
      <h2>Điểm đến nổi bật</h2>
      <div class="destination-list">
        <div class="destination-item">
          <img src="https://www.dulichhalong.net/wp-content/uploads/2022/04/FLC-Grand-Hotel-Halong.jpg" alt="Vịnh Hạ Long" />
          <h3>Vịnh Hạ Long</h3>
          <p>Thiên đường trên biển với những hòn đảo kỳ vĩ.</p>
        </div>
        <div class="destination-item">
          <img src="https://booking.muongthanh.com/upload_images/images/dn1_1654683350.jpg" alt="Đà Nẵng" />
          <h3>Đà Nẵng</h3>
          <p>Thành phố đáng sống với những bãi biển tuyệt đẹp.</p>
        </div>
        <div class="destination-item">
          <img src="https://motortrip.vn/wp-content/uploads/2022/03/khach-san-sapa-21.jpg" alt="Sa Pa" />
          <h3>Sa Pa</h3>
          <p>Vùng đất mờ sương với ruộng bậc thang hùng vĩ.</p>
        </div>
      </div>
    </div> -->
    <div class="destination-section">
    <h2>ĐIỂM ĐẾN NỔI BẬT</h2>
    <div class="destination-list">
      <div class="destination-item">
        <img src="https://booking.muongthanh.com/upload_images/images/H%60/cau-vang-da-nang.jpg" alt="Đà Nẵng">
        <div class="destination-title">Đà Nẵng 🇻🇳</div>
      </div>
      <div class="destination-item">
        <img src="https://bcp.cdnchinhphu.vn/334894974524682240/2024/6/22/screenshot1719044596-1719044886555504330696.png" alt="TP. Hồ Chí Minh">
        <div class="destination-title">TP. Hồ Chí Minh 🇻🇳</div>
      </div>
      <div class="destination-item">
        <img src="https://media-cdn-v2.laodong.vn/Storage/NewsPortal/2022/8/23/1084256/295497942_2922294937.jpg" alt="Hà Nội">
        <div class="destination-title">Hà Nội 🇻🇳</div>
      </div>
      <div class="destination-item">
        <img src="https://cdn.quangnam.gov.vn/2024/09/01/hoi-an.jpg" alt="Hội An">
        <div class="destination-title">Hội An 🇻🇳</div>
      </div>
      <div class="destination-item">
        <img src="https://cdn.tgdd.vn/Files/2021/06/15/1360257/ngat-ngay-voi-5-dia-diem-du-lich-hue-noi-tieng-hap-dan-dep-quen-loi-ve-202306211529096077.jpg" alt="Huế">
        <div class="destination-title">Huế 🇻🇳</div>
      </div>
    </div>
  </div>
    <div class="hotel">
    <h2 class="section-title">Khách sạn nổi bật</h2>
    <div class="hotel-grid">
      <div class="hotel-card">
        <div class="image-wrapper">
          <img src="https://motortrip.vn/wp-content/uploads/2022/03/khach-san-da-nang-4-sao-8.jpg" alt="DLG Hotel" />
          <span class="price-badge">1.000.000 VNĐ/đêm</span>
        </div>
        <div class="hotel-info">
          <h3>DLG Hotel</h3>
          <p>Thành phố Đà Nẵng</p>
        </div>
      </div>
      <div class="hotel-card">
        <div class="image-wrapper">
          <img src="https://booking.muongthanh.com/upload_images/images/dn1_1654683350.jpg" alt="Mường Thanh" />
          <span class="price-badge">1.500.000 VNĐ/đêm</span>
        </div>
        <div class="hotel-info">
          <h3>Mường Thanh Hotel</h3>
          <p>Thành phố Đà Nẵng</p>
        </div>
      </div>
      <div class="hotel-card">
        <div class="image-wrapper">
          <img src="https://www.dulichhalong.net/wp-content/uploads/2022/04/FLC-Grand-Hotel-Halong.jpg" alt="Stark House" />
          <span class="price-badge">1.000.000 VNĐ/đêm</span>
        </div>
        <div class="hotel-info">
          <h3>Stark House</h3>
          <p>Thành phố Hạ Long</p>
        </div>
      </div>
      <div class="hotel-card">
        <div class="image-wrapper">
          <img src="https://www.vietnambooking.com/wp-content/uploads/2021/06/khach-san-5-sao-sai-gon-23.jpg" alt="Bobox" />
          <span class="price-badge">800.000 VNĐ/đêm</span>
        </div>
        <div class="hotel-info">
          <h3>Bobox</h3>
          <p>Thành phố Hồ Chí Minh</p>
        </div>
      </div>
      <div class="hotel-card">
        <div class="image-wrapper">
          <img src="https://image.vietgoing.com/hotel/01/62/vietgoing_sdo2202244107.webp" alt="Ocean Land" />
          <span class="price-badge">2.000.000 VNĐ/đêm</span>
        </div>
        <div class="hotel-info">
          <h3>Ocean Land</h3>
          <p>Thành phố Hồ Chí Minh</p>
        </div>
      </div>
      <div class="hotel-card">
        <div class="image-wrapper">
          <img src="https://vcdn1-dulich.vnecdn.net/2021/05/19/1-1621411309.jpg?w=460&h=0&q=100&dpr=2&fit=crop&s=Qprm1lXgLISL0fUL-abXbQ" alt="Ocean Land" />
          <span class="price-badge">2.000.000 VNĐ/đêm</span>
        </div>
        <div class="hotel-info">
          <h3>Land Hotel</h3>
          <p>Sapa</p>
        </div>
      </div>
      <div class="hotel-card">
        <div class="image-wrapper">
          <img src="https://du-lich.chudu24.com/f/m/2105/19/khach-san-kk-sapa-3.jpg?w=800&h=500" alt="Ocean Land" />
          <span class="price-badge">2.000.000 VNĐ/đêm</span>
        </div>
        <div class="hotel-info">
          <h3>Sapa Hotel</h3>
          <p>Sapa</p>
        </div>
      </div>
      <div class="hotel-card">
        <div class="image-wrapper">
          <img src="https://eholiday.vn/wp-content/uploads/2023/06/Khach-san-Sapa-Legend-Hotel-Spa.jpg" alt="Ocean Land" />
          <span class="price-badge">1.500.000 VNĐ/đêm</span>
        </div>
        <div class="hotel-info">
          <h3>Sapa Legend</h3>
          <p>Sapa</p>
        </div>
      </div>
    </div>
  </div>
  <div class="benefits-section">
    <div class="benefit-item">
      <div class="benefit-icon">
        <img src="https://imgcy.trivago.com//hardcodedimages/homepage-landing/usp/Search.svg" alt="Tìm dễ dàng">
      </div>
      <h3>Tìm dễ dàng</h3>
      <p>Tìm trong số 5 triệu khách sạn chỉ sau vài giây.</p>
    </div>
    <div class="benefit-item">
      <div class="benefit-icon">
        <img src="https://imgcy.trivago.com//hardcodedimages/homepage-landing/usp/Compare.svg" alt="Tự tin so sánh">
      </div>
      <h3>Tự tin so sánh</h3>
      <p>So sánh giá phòng từ nhiều trang web cùng lúc.</p>
    </div>
    <div class="benefit-item">
      <div class="benefit-icon">
        <img src="https://imgcy.trivago.com//hardcodedimages/homepage-landing/usp/Save.svg" alt="Tiết kiệm nhiều">
      </div>
      <h3>Tiết kiệm nhiều</h3>
      <p>Khám phá ưu đãi hấp dẫn để đặt trên trang web đối tác của chúng tôi.</p>
    </div>
  </div>
  <section class="register-accommodation">
    <div class="line"></div>
    <div class="container">
      <!-- Nội dung bên trái -->
      <div class="text-content">
        <h2 class="title">Đăng ký nơi nghỉ của bạn</h2>
        <p class="description">
          Tiếp cận hàng triệu khách hàng tiềm năng và nâng tầm doanh nghiệp
          của bạn với chúng tôi.
        </p>
      </div>

      <!-- Ảnh bên phải -->
      <div class="image-content">
        <img
          src="https://images2.thanhnien.vn/528068263637045248/2024/6/18/4456088079849005103085367538303385702661889n-1718696082415574828640.jpg"
          alt="Phòng khách sạn"
          class="hotel-image"
        />
      </div>
    </div>
    <div class="line"></div>
  </section>
  </div>
</template>
<script setup></script>

<style scoped>
/* Hero Section */
.hero {
  background: #1e3a8a;
  color: white;
  text-align: center;
  padding: 90px 20px;
}

.hero h1 {
  font-size: 28px;
  font-weight: bold;
}

.hero p {
  font-size: 18px;
  margin-top: 10px;
}

.search-box {
  display: flex;
  justify-content: center;
  background: white;
  padding: 20px;
  gap: 20px;
  align-items: flex-end;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  margin: -50px auto 30px;
  max-width: 80%;
  border-radius: 10px;
}

.input-group {
  display: flex;
  flex-direction: column;
  flex: 1;
  min-width: 220px;
}
.input-group label {
  font-weight: bold;
  color: #1e3a8a;
  margin-bottom: 5px;
  font-size: 16px;
}
.input-group input {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  font-size: 14px;
  width: 100%;
}

/* Nút tìm kiếm */
.search-btn {
  background: #e85d04;
  color: white;
  font-size: 16px;
  padding: 12px 24px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  white-space: nowrap;
}

.search-btn:hover {
  background: #d9480f;
}
.destination-section {
  text-align: left;
  margin: 50px auto;
  max-width: 80%;
}

h2 {
  font-size: 24px;
  color: #1e3a8a;
  font-weight: bold;
  text-transform: uppercase;
  position: relative;
  padding-bottom: 10px;
  margin-bottom: 20px;
}

h2::after{
  content: "";
  display: block;
  width: 100%;
  height: 2px;
  background-color: #1e3a8a;
  position: absolute;
  bottom: 0;
  left: 0;
}

.destination-list {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  padding: 0 50px;
}

.destination-item {
  position: relative;
  width: calc(50% - 5px);
  border-radius: 8px;
  overflow: hidden;
}

.destination-item:nth-child(n+3) {
  width: calc(33.33% - 7px);
}

.destination-item img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 8px;
}

.destination-title {
  position: absolute;
  top: 10px;
  left: 10px;
  color: white;
  font-weight: bold;
  font-size: 16px;
  background: rgba(0, 0, 0, 0.5);
  padding: 5px 10px;
  border-radius: 4px;
}
.hotel{
  text-align: left;
  margin: 50px auto;
  max-width: 80%;
}
.section-title {
  font-size: 24px;
  color: #1e3a8a;
  font-weight: bold;
  text-transform: uppercase;
  position: relative;
  padding-bottom: 10px;
  margin-bottom: 20px;
}
.section-title::after{
  content: "";
  display: block;
  width: 100%;
  height: 2px;
  background-color: #1e3a8a;
  position: absolute;
  bottom: 0;
  left: 0;
}
.hotel-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  padding: 0 50px;
}
.hotel-card {
  background: white;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  text-align: center;
}
.image-wrapper {
  position: relative;
}
.image-wrapper img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}
.price-badge {
  position: absolute;
  top: 10px;
  right: 10px;
  background: #1e3a8a;
  color: white;
  padding: 5px 10px;
  border-radius: 5px;
  font-size: 14px;
}
.hotel-info {
  padding: 15px;
}
.hotel-info h3 {
  font-size: 18px;
  font-weight: bold;
  color: #1e3a8a;
}
.hotel-info p {
  font-size: 14px;
  color: #666;
}
.benefits-section {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 40px;
  padding: 30px 10px;
  max-width: 1200px;
  margin: auto;
}

.benefit-item {
  text-align: center;
  max-width: 300px;
}

.benefit-icon {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 120px; /* Điều chỉnh chiều cao để căn giữa */
}

.benefit-item img {
  width: 100px;
  height: auto;
}

.benefit-item h3 {
  font-size: 18px;
  font-weight: bold;
  margin-top: 10px;
}

.benefit-item p {
  font-size: 14px;
  color: #444;
}
.register-accommodation {
  padding: 40px 0;
  background-color: #fff;
}

.line {
  width: 80%;
  margin: 10px auto;
  height: 2px;
  background-color: #1e3a8a;
}

.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: auto;
  gap: 30px;
  padding: 40px 50px;
}

.text-content {
  flex: 1;
}

.title {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}

.description {
  font-size: 16px;
  color: #555;
}

.image-content {
  flex: 1;
}

.hotel-image {
  width: 100%;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}
</style>