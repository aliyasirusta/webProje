<template>
    <div>
     
  
      <!-- Sidebar Menü -->
      <div class="sidebar-container">
        <button class="toggle-btn" @click="toggleSidebar">
          ☰ Menü
        </button>
        <nav class="sidebar" :class="{ open: isSidebarOpen }">
          <!-- Sidebar Kapatma Tuşu -->
          <button class="close-btn" @click="toggleSidebar">✖</button>
          <ul class="menu">
            <!-- Menü Butonları -->
            <li v-for="(button, index) in buttons" :key="index">
              <button @click="currentComponent = index">{{ button }}</button>
            </li>
          </ul>
        </nav>
      </div>
  
      <!-- Ana İçerik -->
      <main>
        
  
        <!-- Components -->
        <component
          v-for="(component, index) in components"
          :key="index"
          :is="component"
          v-show="currentComponent === index"
        />
      </main>
    </div>
  </template>
  
  <script>
  import Component1 from "@/components/Component1.vue";
  import Component2 from "@/components/Component2.vue";
  import Component3 from "@/components/Component3.vue";
  import Component4 from "@/components/Component4.vue";
  import Component5 from "@/components/Component5.vue";
  import Component6 from "@/components/Component6.vue";
  import Component7 from "@/components/Component7.vue";
  import Component8 from "@/components/Component8.vue";
  import Component9 from "@/components/Component9.vue";
  import Component10 from "@/components/Component10.vue";
  
  export default {
    name: "App",
    components: {
      Component1,
      Component2,
      Component3,
      Component4,
      Component5,
      Component6,
      Component7,
      Component8,
      Component9,
      Component10
    },
    data() {
      return {
        isSidebarOpen: false,
        currentComponent: 0, // Başlangıçta görünen komponenti belirler
        components: [
          "Component1", "Component2", "Component3", "Component4", "Component5",
          "Component6", "Component7", "Component8", "Component9", "Component10"
        ],
        buttons: [
          "Ana Sayfanın Üst Bölgesi", "Geçişli Fotoğraf Sekmesi", "Web Sitesi Alt Bilgi Sekmesi", "Ana Ekrandaki Kampanyalar", "Kadın Sweatshirt",
          "Giriş Yapma Bölgesi", "Siparişlerim Sekmesi", "Sepetim", "Favorilerim", "Sürdürebilirlik"
        ],
      };
    },
    methods: {
      toggleSidebar() {
        this.isSidebarOpen = !this.isSidebarOpen;
      },
    },
  };
  </script>
  
  <style scoped>
  /* Logo Alanı */
  .logo-container {
    text-align: center;
    margin: 20px 0;
  }
  
  .logo {
    width: 100px;
    height: auto;
  }
  
  /* Sidebar Konteyner */
  .sidebar-container {
    display: flex;
    align-items: flex-start;
  }
  
  .toggle-btn {
    background-color: #333;
    color: white;
    border: none;
    padding: 10px 15px;
    cursor: pointer;
    font-size: 18px;
    margin-right: 10px;
  }
  
  .toggle-btn:hover {
    background-color: #555;
  }
  
  /* Sidebar */
  .sidebar {
    position: fixed;
    top: 0;
    left: -250px;
    width: 250px;
    height: 100%;
    background-color: #333;
    overflow: hidden;
    transition: all 0.3s ease;
    padding-top: 20px;
    z-index: 1000;
  }
  
  .sidebar.open {
    left: 0; /* Sidebar açık olduğunda */
  }
  
  .menu {
    list-style: none;
    padding: 0;
    margin: 50px 0 0;
  }
  
  .menu li {
    padding: 15px 20px;
  }
  
  .menu button {
    width: 100%;
    padding: 10px;
    background-color: #444;
    color: white;
    border: none;
    cursor: pointer;
    font-size: 5px; /* Yazı boyutunu küçülttüm */
    font-size:10px;
    text-align: left;
  }
  
  .menu button:hover {
    background-color: #555;
  }
  
  /* Kapatma Tuşu */
  .close-btn {
    position: absolute;
    top: 10px;
    right: 10px;
    background: none;
    border: none;
    color: white;
    font-size: 20px;
    cursor: pointer;
  }
  
  .close-btn:hover {
    color: #f0a500;
  }
  
  /* Ana İçerik */
  main {
    margin-left: 260px; /* Sidebar açıkken içerik sola kayar */
    transition: margin-left 0.3s ease;
  }
  
  .sidebar.open + main {
    margin-left: 260px; /* Sidebar açıldığında içerik sola kayar */
  }
  </style>
  