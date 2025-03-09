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
    <section class="tips">
  <h2>Travel Tips</h2>
  <div class="tips-container">
    <div class="tip-box">
      <h3 class="tip-h">Sunny Weather</h3>
      <ul>
        <li>Stay Hydrated: The sun can dehydrate you quickly, so make sure to drink plenty of water throughout the day. Carry a reusable water bottle to refill as needed.</li>
        <li>Wear Sunscreen: Protect your skin from harmful UV rays by applying sunscreen with a high SPF, even on cloudy days. Reapply every 2-3 hours, especially if you're sweating or swimming.</li>
        <li>Dress in Light, Breathable Clothing: Opt for lightweight fabrics like cotton or linen to keep cool. Light-colored clothes will reflect the sun and help prevent overheating.</li>

      </ul>
    </div>

    <div class="tip-box">
      <h3 class="tip-h">Cloudy Weather</h3>
      <ul>
        <li>Light Layers: The temperature can fluctuate, so it's best to wear layers that you can add or remove depending on how warm or cool it feels. A light jacket or sweater will be helpful.</li>
        <li>Pack an Umbrella or Light Rain Jacket: While cloudy weather may not always bring rain, it's always a good idea to be prepared just in case. A compact umbrella or a waterproof jacket can keep you dry if a drizzle arrives.</li>
        <li>Comfortable Shoes: The weather may be a bit unpredictable, so wear shoes that are comfortable for walking, and preferably waterproof in case of light showers.</li>

      </ul>
    </div>

    <div class="tip-box">
      <h3 class="tip-h">Snowy Weather</h3>
      <ul>
        <li>Layer Up: Snowy weather can be very cold, so layering is key. Wear thermal base layers, a warm sweater, and an insulated coat to keep yourself cozy.</li>
        <li>Wear Waterproof Boots: Make sure your shoes are waterproof and have good grip to prevent slipping on icy sidewalks. Insulated boots will also help keep your feet warm.</li>
        <li>Protect Your Skin: Cold, dry air can cause skin to crack and become irritated, so use a rich moisturizer and lip balm to keep your skin hydrated.</li>

      </ul>
    </div>

    <div class="tip-box">
      <h3 class="tip-h">Rainy Weather</h3>
      <ul>
        <li>Pack a Waterproof Jacket and Umbrella: Make sure you have a reliable waterproof jacket and a compact, sturdy umbrella to stay dry while you explore. Choose a jacket with a hood to keep your head dry.</li>
        <li>Choose Waterproof Gear: Look for waterproof or water-resistant shoes, bags, and clothing to stay dry. This will help prevent discomfort and protect your belongings from getting wet.</li>
        <li>Plan for Indoor Activities: While it's always nice to be outside, rainy weather can offer the perfect excuse to check out museums, galleries, or indoor markets. Use the rain as an opportunity to explore the local culture indoors.</li>

      </ul>
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
  margin-top: 50px;
  padding: 40px 20px;
  background-color: #e7f2f8;
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
.tips {
  margin-top: 50px;
  margin-bottom: 100px;
  padding: 40px 20px;
  background-color: #eaf5fb;
  text-align: center;
}

.tips h2 {
  font-size: 2rem;
  margin-bottom: 30px;
  color: #333;
}

.tips-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  gap: 20px;
}

.tip-box {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  width: 280px;
  padding: 20px;
  text-align: left;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.tip-box:hover {
  transform: translateY(-5px);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
}

.tip-h {
  font-size: 1.5rem;
  margin-bottom: 15px;
  color: #242c34;
}

.tip-box ul {
  list-style-type: disc;
  padding-left: 20px;
  margin-bottom: 15px;
  font-size: 1rem;
  line-height: 1.6;
  color: #555;
}

.tip-box ul li {
  margin-bottom: 10px;
}
</style>
