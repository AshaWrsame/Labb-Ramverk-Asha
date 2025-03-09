<template>
  <main>
    <section class="hero">
      <img src="../assets/images/default.jpg" alt="Weather Image">
      <div class="herotext">
        <h1>The Weather att your next travel destination</h1>
        <RouterLink to="/about" class="btn-hero">Get Weather </RouterLink>
      </div>
    </section>
    <section class="destination-container">
      <h2>Travel Suggestions</h2>
      <div class="destinations">
        <div class="destination">
          <img src="../assets/images/paris.jpg" alt="Paris">
          <h3>Paris</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/new-york.jpg" alt="New York">
          <h3>New York</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/tokyo.jpg" alt="Tokyo">
          <h3>Tokyo</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/london.jpg" alt="London">
          <h3>London</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/sydney.jpg" alt="Sydney">
          <h3>Sydney</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/barcelona.jpg" alt="Barcelona">
          <h3>Barcelona</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/rome.jpg" alt="Rome">
          <h3>Rome</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/cape-town.jpg" alt="Cape Town">
          <h3>Cape Town</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/los-angeles.jpg" alt="Los Angeles">
          <h3>Los Angeles</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/amsterdam.jpg" alt="Amsterdam">
          <h3>Amsterdam</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/berlin.webp" alt="Berlin">
          <h3>Berlin</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/kyoto.jpg" alt="Kyoto">
          <h3>Kyoto</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/bali.webp" alt="Bali">
          <h3>Bali</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/maldives.jpg" alt="Maldives">
          <h3>Maldives</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/hawaii.jpg" alt="Hawaii">
          <h3>Hawaii</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/mauritius.jpg" alt="Mauritius">
          <h3>Mauritius</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/sri-lanka.jpg" alt="Sri Lanka">
          <h3>Sri Lanka</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/fiji.jpg" alt="Fiji">
          <h3>Fiji</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/costa-rica.jpg" alt="Costa Rica">
          <h3>Costa Rica</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/zanzibar.jpg" alt="Zanzibar">
          <h3>Zanzibar</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/phuket.jpg" alt="Phuket">
          <h3>Phuket</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/seychelles.jpg" alt="Seychelles">
          <h3>Seychelles</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/bora-bora.png" alt="Bora Bora">
          <h3>Bora Bora</h3>
        </div>
        <div class="destination">
          <img src="../assets/images/boracay.jpg" alt="Boracay">
          <h3>Boracay</h3>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
</script>

<style scoped>
.hero {
  position: relative;
  width: 100%;
  height: 40vh;
  overflow: hidden;
}

.hero img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.herotext {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  color: white;
}

.herotext h1 {
  font-size: 2.5rem;
  margin-bottom: 20px;
}

.btn-hero {
  padding: 10px 20px;
  font-size: 1rem;
  background-color: white;
  color: black;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.btn-hero:hover {
  background-color: #f0f0f0;
}
.destination-container {
  padding: 40px 20px;
  background-color: #f9f9f9;
  text-align: center;
}

.destination-container h2 {
  font-size: 2rem;
  margin-bottom: 30px;
}

.destinations {
  display: flex;
  animation: scrollDestinations 30s linear infinite;
}

.destination {
  margin: 0 15px;
  text-align: center;
  width: 250px;
}

.destination img {
  width: auto;
  height: 150px;
  object-fit: cover;
  border-radius: 2px;
}

.destination h3 {
  margin-top: 10px;
  font-size: 1.5rem;
  color: #333;
}

@keyframes scrollDestinations {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-50%);
  }
}
</style>
