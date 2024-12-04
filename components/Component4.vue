<template>
    <div class="image-grid">
      <!-- Üstteki iki görsel -->
      <div class="image-item large">
        <img src="https://ktnimg2.mncdn.com/cms/2024/11/27/c91eb507-b4db-4bff-bf49-acb96615873d.png" alt="Dış Giyim" />
        <div class="overlay">
          <h3>Dış Giyim</h3>
          <a href="#">ALIŞVERİŞE BAŞLA</a>
        </div>
      </div>
      <div class="image-item large">
        <img src="https://ktnimg2.mncdn.com/cms/2024/11/27/42c8f1b2-02ad-4217-bbd6-f130e3eeb012.png" alt="Dış Giyim" />
        <div class="overlay">
          <h3>Dış Giyim</h3>
          <a href="#">ALIŞVERİŞE BAŞLA</a>
        </div>
      </div>
  
      <!-- Orta görsel -->
      <div class="image-item wide">
        <img src="https://ktnimg2.mncdn.com/cms/2024/11/27/cc8f9c12-9f26-45c7-8e9d-03dd3cc69688.png" alt="Kazak & Süveter" />
        <div class="overlay">
          <h3>Kazak & Süveter</h3>
          <a href="#">ALIŞVERİŞE BAŞLA</a>
        </div>
      </div>
  
      <!-- Alttaki dört görsel -->
      <div class="image-item small">
        <img src="https://ktnimg2.mncdn.com/cms/2024/11/27/67be0185-1096-4874-a85a-0e20f22cbc8c.png" alt="Jean" />
        <div class="overlay">
          <h3>Jean</h3>
          <a href="#">ALIŞVERİŞE BAŞLA</a>
        </div>
      </div>
      <div class="image-item small">
        <img src="https://ktnimg2.mncdn.com/cms/2024/11/27/c1239eab-11de-41db-a33a-8ada7e89e50f.png" alt="Parti Elbisesi" />
        <div class="overlay">
          <h3>Parti Elbisesi</h3>
          <a href="#">ALIŞVERİŞE BAŞLA</a>
        </div>
      </div>
      <div class="image-item small">
        <img src="https://ktnimg2.mncdn.com/cms/2024/11/27/79c41330-8783-4467-841f-8600c69c0926.png" alt="Hırka" />
        <div class="overlay">
          <h3>Hırka</h3>
          <a href="#">ALIŞVERİŞE BAŞLA</a>
        </div>
      </div>
      <div class="image-item small">
        <img src="https://ktnimg2.mncdn.com/cms/2024/11/27/bbedb8f4-3abd-4c53-ad15-fe8a1b99e43e.png" alt="Sweatshirt" />
        <div class="overlay">
          <h3>Sweatshirt</h3>
          <a href="#">ALIŞVERİŞE BAŞLA</a>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Component4",
  };
  </script>
  
  <style scoped>
  .image-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 10px;
    margin: 20px;
  }
  
  .image-item {
    position: relative;
    overflow: hidden;
  }
  
  .image-item img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }
  
  /* Overlay tasarımı */
  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    opacity: 0;
    transition: opacity 0.3s ease;
  }
  
  .overlay h3 {
    font-size: 18px;
    margin-bottom: 10px;
  }
  
  .overlay a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    border: 1px solid white;
    padding: 5px 10px;
    border-radius: 3px;
  }
  
  .image-item:hover .overlay {
    opacity: 1;
  }
  
  /* Boyutlandırmalar */
  .large {
    grid-column: span 2; /* Büyük resimler için */
    height: 300px;
  }
  
  .wide {
    grid-column: span 4; /* Orta geniş resim için */
    height: 400px;
  }
  
  .small {
    grid-column: span 1; /* Küçük resimler */
    height: 200px;
  }
  </style>
  