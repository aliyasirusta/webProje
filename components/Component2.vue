<template>
    <div class="slider-container" @click="nextImage">
      <!-- Resim -->
      <div class="image-container">
        <img :src="images[currentImageIndex]" alt="Slider Image" class="slider-image" />
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Component2",
    data() {
      return {
        images: [
          "https://ktnimg2.mncdn.com/cms/2024/11/13/6a7a1ccf-dbe7-4fb6-b527-b9c6c28fe860.png",
          "https://ktnimg2.mncdn.com/cms/2024/11/26/485c50ba-9a72-46e8-b8b9-95fc1c83cbd5.jpg",
          
          "https://ktnimg2.mncdn.com/cms/2024/11/26/253859e2-913c-44c9-98d3-2f203dddc91f.jpg",
          
        ],
        currentImageIndex: 0, // Şu anda gösterilen resmin index'i
      };
    },
    methods: {
      nextImage() {
        // Resme tıklandığında bir sonraki resme geçer
        this.currentImageIndex =
          (this.currentImageIndex + 1) % this.images.length;
      },
    },
  };
  </script>
  <style scoped>
  /* Slider Konteyner */
  .slider-container {
  position: relative;
  width: 90%; /* Daha geniş bir slider */
  max-width: 1000px; /* Maksimum genişlik sınırı */
  margin: 60px auto; /* Yukarıdan boşluk eklemek için margin-top ayarlandı */
  text-align: center;
  overflow: hidden;
  cursor: pointer; /* Tıklanabilir olduğunu belirtmek için */
}
  
  /* Resim Konteyneri */
  .image-container {
    position: relative;
    width: 100%;
    height: 500px; /* Daha yüksek bir alan */
  }
  
  .slider-image {
    width: 100%;
    height: 100%;
    object-fit: contain; /* Resimlerin tamamını gösterir */
    border-radius: 15px; /* Hafif bir köşe yuvarlaması */
    transition: transform 0.3s ease; /* Hafif bir animasyon ekler */
  }
  
  .slider-container:hover .slider-image {
    transform: scale(1.02); /* Hover efektini biraz küçülttüm */
  }
  </style>