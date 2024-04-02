<!-- Navbar.vue -->
<template>
  <nav>
    <ul>
      <router-link to="/">Home</router-link>
      <router-link to="/profil">Profil</router-link>
      <router-link to="/hobby">Hobby</router-link>
    </ul>
  </nav>
  <div id="app">
    <Navbar />
    <router-view></router-view>
    
  <div class="navbar-content">
    <img src="../src/assets/fotocontent.jpg">
    <h1>EBBY ARRAHMAN TARIF</h1>
    <h2>TEKNIK INFORMATIKA</h2>
    <h3>4C</h3>

    <div class="konten-grid">
        <div class="konten">
          <img src="../src/assets/calisthenic.jpg">
          <p>Calisthenic</p>
        </div>
        <div class="konten">
          <img src="../src/assets/berenang.jpg">
          <p>Berenang</p>
        </div>
        <div class="konten">
          <img src="../src/assets/game.jpg">
          <p>Game Mobile Legend</p>
        </div>
        <div class="konten">
          <img src="../src/assets/gunung.jpg">
          <p>Mendaki Gunung</p>
        </div>
      </div>
  </div>
  <footer>
      <p>&copy; 2024 - Ebby Arrahman Tarif</p>
    </footer>
  </div>
</template>

<style scoped>
/* Styling khusus untuk komponen Navbar */
nav {
  background-color: #dd8d24;
  padding: 10px 0;
}

ul {
  list-style-type: none;
  text-align: center;
}

li {
  display: inline;
}

router-link {
  color: #0d0d0e;
  text-decoration: none;
  padding: 25px 50px;
}

router-link:hover {
  background-color: #efecf1;
}

/* Styling untuk konten dalam navbar */
.navbar-content {
  color: #f8f3f3;
  text-align: center;
  margin-top: 20px;
  
}

/* Styling untuk gambar */
.navbar-content img {
  width: 200px; /* Atur lebar gambar sesuai kebutuhan */
  height: 200px; /* Tinggi gambar akan disesuaikan agar tidak terlalu terdistorsi */
  margin-bottom: 10px; /* Jarak antara gambar dengan teks di bawahnya */
  border-radius: 50%;
}

#app {
  background-image: url('../src/assets/backgroundUniversal.jpg'); /* Ganti dengan path file gambar Anda */
  background-size: cover;
  background-position: center;
  min-height: 100vh; /* Untuk memastikan background mengisi seluruh tinggi layar */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
  .konten-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr); /* Membuat 4 kolom dengan lebar yang sama */
  gap: 20px; /* Jarak antara kolom */
}

/* Styling untuk konten dalam kolom */
.konten {
  background-color: rgba(68, 66, 66, 0.8); /* Warna latar belakang dengan transparansi */
  padding: 1px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Efek bayangan untuk konten */
}

/* Styling untuk footer */
footer {
  background-color: #333;
  color: #fff;
  text-align: center;
  width: 1325px; /* Atur lebar gambar sesuai kebutuhan */
  height: 50px; /* Tinggi gambar akan disesuaikan agar tidak terlalu terdistorsi */
}

</style>
