<template>
    <div class="cart-page">
      <div class="cart-items">
        <h1>Sepetim</h1>
        <ul>
          <li v-for="item in cartItems" :key="item.id" class="cart-item">
            <img :src="item.image" alt="Ürün görseli" class="item-image" />
            <div class="item-details">
              <h2>{{ item.name }}</h2>
              <p><strong>Renk:</strong> {{ item.color }}</p>
              <p><strong>Beden:</strong> {{ item.size }}</p>
              <button class="edit-button">Düzenle</button>
            </div>
            <div class="item-actions">
              <select v-model="item.quantity">
                <option v-for="n in 10" :key="n" :value="n">{{ n }}</option>
              </select>
              <p class="item-price">{{ item.price }} TL</p>
              <button class="remove-button" @click="removeItem(item.id)">✖</button>
            </div>
          </li>
        </ul>
      </div>
      <div class="cart-summary">
        <h2>Sipariş Özeti</h2>
        <p><strong>Ürünlerin Toplamı:</strong> {{ totalBeforeDiscount }} TL</p>
        <p><strong>Toplam İndirim:</strong> {{ totalDiscount }} TL</p>
        <p><strong>Toplam:</strong> {{ totalAfterDiscount }} TL</p>
        <input type="text" placeholder="Promosyon Kodu" class="promo-code-input" />
        <button class="promo-code-button">EKLE</button>
        <button class="checkout-button">SİPARİŞİ TAMAMLA</button>
        <button class="fast-checkout-button">HIZLI ÖDE</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        cartItems: [
          {
            id: 1,
            name: "Slim Fit Kaşe Kaban Cep Detaylı",
            color: "GRİ",
            size: "S",
            image: "https://ktnimg2.mncdn.com/products/2024/11/11/2942979/65087145-53f3-41b6-9755-49c59cad2814_size240x314.jpg", // Ürün resmi için bir URL ekleyin
            price: 2699.99,
            quantity: 1,
          },
          {
            id: 2,
            name: "Oversize Kot Ceket Crop Boy",
            color: "KOYU İNDİGO",
            size: "XL",
            image: "https://ktnimg2.mncdn.com/products/2024/10/25/2994023/659a7f8a-6a89-46ce-9df7-5314243e66c6_size240x314.jpg",
            price: 1499.99,
            quantity: 1,
          },
          {
            id: 3,
            name: "Super Baggy Kot Pantolon",
            color: "KOYU İNDİGO",
            size: "32",
            image: "https://ktnimg2.mncdn.com/products/2024/10/25/2994025/1ac7bf04-c733-439d-aec1-1f1160bf27ca_size240x314.jpg  ",
            price: 1099.99,
            quantity: 1,
          },
          {
            id: 4,
            name: "Basic Triko Kazak Uzun Kollu",
            color: "VİZON",
            size: "M",
            image: "https://ktnimg2.mncdn.com/products/2024/08/09/2970322/e1ab99a8-fba6-4817-b9bb-f9836ad641ba_size240x314.jpg",
            price: 729.99,
            quantity: 1,
          },
        ],
      };
    },
    computed: {
      totalBeforeDiscount() {
        return this.cartItems.reduce((sum, item) => sum + item.price * item.quantity, 0).toFixed(2);
      },
      totalDiscount() {
        return (this.totalBeforeDiscount * 0.3).toFixed(2); // %30 indirim örneği
      },
      totalAfterDiscount() {
        return (this.totalBeforeDiscount - this.totalDiscount).toFixed(2);
      },
    },
    methods: {
      removeItem(id) {
        this.cartItems = this.cartItems.filter(item => item.id !== id);
      },
    },
  };
  </script>
  
  <style scoped>
  .cart-page {
    display: flex;
    justify-content: space-between;
    font-family: Arial, sans-serif;
    padding: 20px;
  }
  
  .cart-items {
    flex: 3;
    margin-right: 20px;
  }
  
  .cart-item {
    display: flex;
    align-items: center;
    border-bottom: 1px solid #ddd;
    padding: 10px 0;
  }
  
  .item-image {
    width: 100px;
    height: auto;
    margin-right: 20px;
  }
  
  .item-details {
    flex: 2;
  }
  
  .item-actions {
    flex: 1;
    text-align: right;
  }
  
  .edit-button,
  .remove-button {
    background: none;
    border: none;
    color: #ff6200;
    cursor: pointer;
    margin-top: 5px;
  }
  
  .remove-button {
    font-size: 20px;
    color: red;
  }
  
  .cart-summary {
    flex: 1;
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 5px;
  }
  
  .cart-summary h2 {
    margin-bottom: 20px;
  }
  
  .promo-code-input {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ddd;
    border-radius: 5px;
  }
  
  .promo-code-button,
  .checkout-button,
  .fast-checkout-button {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  
  .checkout-button {
    background-color: #000;
    color: #fff;
  }
  
  .fast-checkout-button {
    background-color: red;
    color: #fff;
  }
  </style>
  