<template>
    <div class="component">
      <!-- Üst Başlık ve Logo -->
      <p class="greeting">Sürpriz Kupon Fırsatları İçin Tıkla</p> 
      <div class="top-bar">
        <!-- Sol Menü Yazıları -->
        <div class="menu-container">
          <span class="menu-item">Kadın
            <!-- Kadın alt kategoriler -->
            <div class="submenu">
      <span class="submenu-item">Yeni Gelenler</span>
      <span class="submenu-item">Çok Satanlar</span>
      <span class="submenu-item">Giyim
        <!-- Giyim alt kategorileri yeni bar -->
        <div class="submenu1">
          <span class="submenu1-item">Tüm Ürünler</span>
          <span class="submenu1-item">Dış Giyim</span>
          <span class="submenu1-item">Kaban</span>
          <span class="submenu1-item">Mont</span>
          <span class="submenu1-item">Peluş Mont</span>
          <span class="submenu1-item">Sweatshirt</span>
          <span class="submenu1-item">Kazak & Süveter</span>
          <span class="submenu1-item">Triko Sıcaklığı</span>
          <span class="submenu1-item">Hırka</span>
          <span class="submenu1-item">Elbise</span>
          <span class="submenu1-item">Yelek</span>
          <span class="submenu1-item">Etek</span>
          <span class="submenu1-item">Pantolon</span>
          <span class="submenu1-item">Ceket</span>
          <span class="submenu1-item">Suni Deri Ceket</span>
          <span class="submenu1-item">Blazer Ceket</span>
          <span class="submenu1-item">Gömlek</span>
          <span class="submenu1-item">Bluz</span>
          <span class="submenu1-item">Trençkot</span>
          <span class="submenu1-item">Abiye Davet</span>
          <span class="submenu1-item">Crop</span>
          <span class="submenu1-item">Top/Bluz</span>
          <span class="submenu1-item">Tişört</span>
          <span class="submenu1-item">Eşofman Altı</span>
          <span class="submenu1-item">Tayt</span>
          <span class="submenu1-item">Pijama Takımı</span>
          <span class="submenu1-item">Koton Jeans</span>
          <span class="submenu1-item">Kot Pantolon</span>
          <span class="submenu1-item">Kot Ceket</span>
          <span class="submenu1-item">Tişört Uzun Kol</span>
        </div>
      </span>
      <span class="submenu-item">Genç Kadın</span>
      <span class="submenu-item">Koleksiyonlar</span>
      <span class="submenu-item">Abiye & Davet</span>
      <span class="submenu-item">İç Giyim ve Pijama</span>
      <span class="submenu-item">Spor Giyim</span>
      <span class="submenu-item">Aksesuar</span>
    </div>
          </span>
          <span class="menu-item">Erkek</span>
          <span class="menu-item">Çocuk</span>
          <span class="menu-item">Bebek</span>
          <span class="menu-item">Jeans</span>
          <span class="menu-item">Trend Kasım</span>
          <span class="menu-item">Sürpriz Kupon</span>
          <span class="menu-item">Sürdürülebilirlik</span>
        </div>
  
        <!-- Logo ve Yazı (Ortada) -->
        <div class="logo-container">
          <img src="https://lh6.googleusercontent.com/proxy/x-IowmB16zm7DUjyn4onFnmoToG1L5PX48QSH3FYghgOrMofjQPO7_F-2W73v6zHaEbE_wwnKx807BaIHMqCXcMplROCTy95ssCg" alt="Logo" class="logo" />
        </div>
  
        <!-- Sağ Butonlar -->
        <div class="right-side">
          <!-- Arama Barı -->
          <input type="text" class="search-bar" placeholder="Ara..." />
          <span class="right-item">Koton</span>
          <span class="right-item">Dil</span>
          <span class="right-item account-menu">
          Hesabım
          <div class="submenu">
            <span class="submenu-item">Giriş Yap</span>
            <span class="submenu-item">Kayıt Ol</span>
          </div>
        </span>
         
          <div class="favorites">
  <img src="https://w7.pngwing.com/pngs/501/448/png-transparent-favourite-chart-favorites-heart-rating-top-web-icon-thumbnail.png" alt="Favoriler Logo" class="favorites-logo">
</div>
          <span class="right-item">Siparişlerim</span>
           <!-- Sepetim -->
        <div class="cart-container">
          <span class="cart-text">
            <img src="https://e7.pngegg.com/pngimages/542/31/png-clipart-shopping-cart-shopping-bags-trolleys-computer-icons-shop-text-rectangle.png" alt="Sepet İkonu" class="cart-icon" />          
          </span>
          <div class="cart-dropdown">
            <p class="cart-title">Sepetinizde 4 ürün var</p>
            <ul class="cart-items">
              <li class="cart-item">
                <img src="https://ktnimg2.mncdn.com/products/2024/11/11/2942979/65087145-53f3-41b6-9755-49c59cad2814_size300x390_cropCenter.jpg" alt="Ürün 1" class="cart-item-image" />
                <div class="cart-item-info">
                  <p class="cart-item-name">Slim Fit Kaşe Kaban</p>
                  <p class="cart-item-price">2.699,99 TL</p>
                </div>
              </li>
              <li class="cart-item">
                <img src="https://ktnimg2.mncdn.com/products/2024/10/25/2994023/659a7f8a-6a89-46ce-9df7-5314243e66c6_size300x390_cropCenter.jpg" alt="Ürün 2" class="cart-item-image" />
                <div class="cart-item-info">
                  <p class="cart-item-name">Oversize Kot Ceket</p>
                  <p class="cart-item-price">1.499,99 TL</p>
                </div>
              </li>
              <li class="cart-item">
                <img src="https://ktnimg2.mncdn.com/products/2024/10/25/2994025/1ac7bf04-c733-439d-aec1-1f1160bf27ca_size300x390_cropCenter.jpg" alt="Ürün 3" class="cart-item-image" />
                <div class="cart-item-info">
                  <p class="cart-item-name">Triko Kazak</p>
                  <p class="cart-item-price">599,99 TL</p>
                </div>
              </li>
              <li class="cart-item">
                <img src="https://ktnimg2.mncdn.com/products/2024/08/09/2970322/e1ab99a8-fba6-4817-b9bb-f9836ad641ba_size300x390_cropCenter.jpg" alt="Ürün 4" class="cart-item-image" />
                <div class="cart-item-info">
                  <p class="cart-item-name">Deri Ceket</p>
                  <p class="cart-item-price">1.200,00 TL</p>
                </div>
              </li>
            </ul>
            <div class="cart-total">
              <p>Toplam: <strong>4.220,96 TL</strong></p>
            </div>
            <button class="checkout-button">Siparişi Tamamla</button>
          </div>
        </div>
        </div>
      </div>     
    </div>
  </template>
  
  <script>
  export default {
    name: "Component1"
  };
  </script>
  
  <style scoped>
  .favorites {
  display: flex;
  align-items: center;  /* Logoyu ve metni dikeyde ortalar */
}

.favorites-logo {
  width: 20px;  /* Logonun genişliğini ayarlayın */
  height: auto;  /* Yüksekliği orantılı olarak ayarlayın */
  margin-right: 10px;  /* Logonun sağında biraz boşluk bırakın */
}

  /* Sepetim Dropdown */
.cart-container {
  position: relative;
}
.cart-container {
  position: relative;
}

.cart-text {
  color: white;
  font-size: 12px;
  cursor: pointer;
  font-weight: bold;
  text-transform: uppercase;
}
.cart-icon {
  width: 20px;
  height: 20px;
  margin-right: 5px;
}

.cart-dropdown {
  display: none;
  position: absolute;
  top: 100%;
  right: 0;
  width: 300px;
  background-color: white;
  border: 1px solid #ccc;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  padding: 10px;
  z-index: 1000;
}

.cart-dropdown ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.cart-dropdown ul li {
  padding: 5px 0;
  border-bottom: 1px solid #eee;
}

.checkout-button {
  display: block;
  width: 100%;
  padding: 10px;
  background-color: #f0a500;
  border: none;
  border-radius: 5px;
  color: white;
  font-weight: bold;
  cursor: pointer;
  text-align: center;
}

.checkout-button:hover {
  background-color: #d08a00;
}

/* Sepet Hover */
.cart-container:hover .cart-dropdown {
  display: block;
}
  /* Sayfanın en üstündeki "Selam" yazısı */
  .greeting {
    text-align: right; /* Yazıyı sağa hizalar */
    font-size: 15px;
    font-weight: bold;
    color: #000000;
    margin-top: 2px;
    margin-right: 475px; /* Sağdan biraz boşluk bırakmak için */
    margin-bottom: 0;
  }
  /* Kadın menüsünün altındaki kategori barı (submenu) gizli */
.submenu {
  display: none; /* Başlangıçta gizli */
  position: absolute;
  top: 100%;
  left: 0;
  background-color: #fbfbfb;
  border-radius: 4px;
  padding: 5px 0;
  z-index: 1;
  width: 200px;
}

/* Kadın menüsünün altındaki kategori barı (submenu) görünür */
.menu-item:hover .submenu {
  display: block; /* Kadın menüsüne hover yapıldığında alt menü gösterilsin */
}

/* Giyim alt menüsünün görünür olacağı kurallar */
.submenu1 {
  display: none; /* Başlangıçta gizli */
  position: absolute;
  top: 0;
  left: 100%; /* Giyim'in sağında göstermek için */
  background-color: #fefefe;
  border-radius: 4px;
  padding: 5px 0;
  z-index: 2;
  width: 200px;
}

/* Giyim alt menüsüne hover yapılınca göster */
.submenu-item:hover .submenu1 {
  display: block; /* Giyim alt menüsüne hover yapıldığında daha fazla kategori göster */
}


/* Submenu-item hover */
.submenu-item:hover {
  background-color: #f0a500; /* Hover durumunda alt menü elemanlarının arkaplan rengi değişir */
  color: #040404;
}

.submenu1-item {
  color: rgb(0, 0, 0);
  font-size: 10px;
  padding: 8px 10px;
  cursor: pointer;
  transition: background-color 0.3s;
  display: block;
}

.submenu1-item:hover {
  background-color: #f0a500;
  color: #000000;
}
  /* Üst Başlık ve Logo Konteyneri */
  .top-bar {
    display: flex;
    align-items: center; /* Her öğeyi dikeyde ortala */
    justify-content: space-between; /* Sol menü ve sağ butonlar arasındaki mesafeyi eşitle */
    width: 100%; /* Tüm genişlik kullanılsın */
    padding: 5px 5px; /* Üstte biraz boşluk bırak */
    background-image: url('https://ktnimg2.mncdn.com/cms/2024/11/13/6a7a1ccf-dbe7-4fb6-b527-b9c6c28fe860.png');
    background-size: 1300px 600px; /* Genişlik 400px, yükseklik 200px */
    border-radius: 4px; /* Kenarları yuvarlamak için */
    transition: background-color 0.3s; /* Arka plan renginin geçiş efekti */
  }
  
  /* Logo ve Yazı */
  .logo-container {
    display: flex;
    flex-direction: column; /* Logo ve yazıyı dikey hizalama */
    align-items: center; /* Ortada hizalama */
    flex-grow: 1; /* Genişlik içinde ortalanmasını sağlar */
    margin-left: 0px; /* Logo ile sol menü arasındaki boşluğu kısıtlamak için */
    margin-right: 0px; /* Logo ile sağ butonlar arasındaki boşluğu kısıtlamak için */
  }
  
  .logo {
    width: 90px; /* Logoyu küçültmek için */
    height: auto;
  }
  
  /* Menü Yazıları */
  .menu-container {
    display: flex;
    justify-content: flex-start; /* Menüleri sola hizala */
    flex-wrap: wrap; /* Eğer butonlar çoksa satırlara geçmesini sağlar */
    padding: 2px 2px; /* Menüye iç boşluk eklemek için */
  }
  
  /* Menü Elemanları */
  .menu-item {
    position: relative; /* Alt menünün konumlandırılması için gerekli */
    color: white;
    font-size: 10px; /* Font boyutunu küçültmek için */
    margin: 2px 8px; /* Butonlar arasında mesafe */
    cursor: pointer;
    text-transform: uppercase; /* Yazıyı büyük yapmak için */
    font-weight: bold;
    transition: background-color 0.3s, color 0.3s; /* Renk değişimini yumuşatmak için */
  }
  
  /* Kadın menüsünün altındaki kategori barı (submenu) gizli */
.submenu {
  display: none; /* Başlangıçta gizli */
  position: absolute;
  top: 100%;
  left: 0;
  background-color: #fefefe;
  border-radius: 4px;
  padding: 5px 0;
  z-index: 1; /* Üstte görünmesini sağlar */
  width: 200px; /* Alt menü genişliği */
}
  
  /* Submenu Item (Alt menü elemanları) */
  .submenu-item {
  color: rgb(6, 6, 6);
  font-size: 10px;
  padding: 8px 10px; /* Dikeyde daha geniş bir padding ekleyelim */
  cursor: pointer;
  transition: background-color 0.3s;
  display: block; /* Alt menü öğelerinin alt alta sıralanması için block yapalım */
}
  
  .submenu-item:hover {
    background-color: #f0a500; /* Hover durumunda alt menü elemanlarının arkaplan rengi değişir */
    color: #333;
  }
  /* Kadın Menü Elemanına Hover Yapıldığında Alt Menüyü Göster */
  .menu-item:hover .submenu {
  display: block; /* Alt menüyü görünür hale getirir */
}
.account-menu:hover .submenu {
  display: block;
}
/* Giyim Alt Menü Elemanına Hover Yapıldığında Alt Menüyü Göster */
.submenu-item:hover .submenu {
  display: block; /* Giyim alt menüsüne hover yapıldığında daha fazla kategori göster */
}
  
  /* Sağ Taraf Yazıları */
  .right-side {
    display: flex;
    justify-content: flex-end; /* Sağ tarafa hizala */
    align-items: center; /* Arama barı ve butonları dikeyde hizala */
  }
  
  /* Arama Barı */
  .search-bar {
    width: 120px; /* Genişliği küçülttüm */
    padding: 5px;
    margin-right: 10px;
    border-radius: 5px;
    border: 1px solid #ccc;
    font-size: 12px;
  }
  
  /* Sağ Taraf Elemanları */
  .right-item {
    color: rgb(255, 255, 255);
    font-size: 12px; /* Font boyutunu küçültmek için */
    margin: 2px 8px; /* Butonlar arasında mesafe */
    cursor: pointer;
    text-transform: uppercase; /* Yazıyı büyük yapmak için */
    font-weight: bold;
    transition: background-color 0.3s, color 0.3s; /* Renk değişimini yumuşatmak için */
  }
  
  /* Sağ Taraf Elemanının Üzerine Gelindiğinde Değişen Arka Plan */
  .right-item:hover {
    background-color: #f0a500; /* Hover durumunda arkaplan rengi değişir */
    color: #000000; /* Yazı rengini değiştirmek */
  }
  
  /* Tüm Üst Barın Üzerine Gelindiğinde Renk Değişimi */
  .top-bar:hover {
    background-color: #d8b2b2; /* Üst barın arka plan rengini değiştirme */
  }
  /* Hesabım Alt Menü */
.account-menu {
  position: relative;}
  </style>
  