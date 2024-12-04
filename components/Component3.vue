<template>
  <footer class="footer-container">
    <!-- Üst Bilgi -->
    <div class="footer-top">
      <div class="icon-container">
        <div class="icon-item">Koton Club</div>
        <div class="icon-item">Mağazadan Gel-Al</div>
        <div class="icon-item">Kapıda Ödeme</div>
        <div class="icon-item">Bir Tıkla Kapında</div>
        <div class="icon-item">Güvenli Alışveriş</div>
        <div class="icon-item">Ücretsiz İade</div>
      </div>
    </div>

    <!-- Orta Bilgi -->
    <div class="footer-middle">
      <div class="newsletter">
        <h3>En güncel moda haberleri için kaydolun</h3>
        <p>Herkesten önce kaçırılmaması gereken haberleri alın.</p>
        <div class="newsletter-input">
          <input type="email" placeholder="E-posta" />
          <button>→</button>
        </div>
      </div>
      <div class="mobile-app">
        <h3>Alışveriş Uygulamamızı İndirin</h3>
        <p>Mobil uygulamamızı keşfedin, size özel fırsatları yakalayın!</p>
        <div class="app-buttons">
          <button class="app-button">App Store</button>
          <button class="app-button">Google Play</button>
        </div>
      </div>
    </div>

    <!-- Alt Bilgi -->
    <div class="footer-bottom">
      <div class="footer-links">
        <h4>Kurumsal</h4>
        <ul>
          <li>Hakkımızda</li>
          <li>Koton Blog</li>
          <li>Kurumsal</li>
          <li>İletişim</li>
        </ul>
      </div>
      <div class="footer-links">
        <h4>Yardım</h4>
        <ul>
          <li>Sık Sorulan Sorular</li>
          <li>İade Politikası</li>
          <li>Kampanyalar</li>
        </ul>
      </div>
      <div class="footer-links">
        <h4>Popüler Kategoriler</h4>
        <ul>
          <li>Koton Kadın</li>
          <li>Koton Erkek</li>
          <li>Çocuk Giyim</li>
        </ul>
      </div>
    </div>

    <!-- Sosyal Medya -->
    <div class="footer-social">
      <p>Bizi Takip Edin:</p>
      <div class="social-icons">
        <span>Facebook</span>
        <span>Instagram</span>
        <span>Twitter</span>
        <span>YouTube</span>
      </div>
    </div>
  </footer>
</template>

<style scoped>
/* Genel Konteyner */
.footer-container {
  background-color: #f9f9f9;
  padding: 20px;
  font-family: Arial, sans-serif;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin-top: 10px; /* Ekranın altına boşluk bırakır */
  position: relative; /* İçeriği düzgün hizalamak için */
}

/* Üst Bilgi */
.footer-top {
  display: flex;
  justify-content: space-around;
  padding: 15px 0;
  background-color: #fff;
  border-bottom: 1px solid #ddd;
}

.icon-container {
  display: flex;
  justify-content: space-around;
  width: 100%;
}

.icon-item {
  text-align: center;
  font-size: 14px;
  color: #333;
  padding: 5px;
}

/* Orta Bilgi */
.footer-middle {
  display: flex;
  justify-content: space-between;
  padding: 20px 0;
}

.newsletter,
.mobile-app {
  width: 45%;
}

.newsletter-input {
  display: flex;
  margin-top: 10px;
}

.newsletter-input input {
  flex: 1;
  padding: 5px;
  border: 1px solid #ddd;
}

.newsletter-input button {
  padding: 5px 15px;
  background-color: black;
  color: white;
  border: none;
}

.app-buttons {
  margin-top: 10px;
}

.app-button {
  background-color: #444;
  color: white;
  border: none;
  padding: 5px 15px;
  margin-right: 5px;
}

/* Alt Bilgi */
.footer-bottom {
  display: flex;
  justify-content: space-around;
  background-color: #fff;
  padding: 20px 0;
  border-top: 1px solid #ddd;
}

.footer-links h4 {
  font-size: 16px;
  color: #000;
}

.footer-links ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.footer-links ul li {
  font-size: 14px;
  color: #555;
  margin-bottom: 5px;
}

/* Sosyal Medya */
.footer-social {
  text-align: center;
  margin-top: 20px;
}

.social-icons span {
  margin: 0 10px;
  font-size: 14px;
  color: #333;
}
</style>
