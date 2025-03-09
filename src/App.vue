
<script setup>
import { RouterView } from 'vue-router';
</script>

<template>
  <nav class="navbar">
    <div class="container">
      <ul class="navbar-list">
        <li class="navbar-item">
          <router-link to="/" class="navbar-link">Home</router-link>
        </li>
        <li class="navbar-item">
          <router-link to="/about" class="navbar-link">About</router-link>
        </li>

      </ul>
    </div>
  </nav>
  <footer class="footer">
    <div class="container">
      <p class="footer-text">© 2025 MyWebsite. All rights reserved.</p>
    </div>
  </footer>
  <RouterView/>
</template>

<style scoped>
.navbar {
  background-color: rgba(51, 51, 51, 0.5); /* Dark gray with 70% opacity */
  padding: 10px 0;
}

.navbar .container {
  width: 80%;
  margin: 0 auto;
}

.navbar-list {
  list-style-type: none;
  display: flex;
  justify-content: space-around;
  padding: 0;
}

.navbar-item {
  margin: 0 15px;
}

.navbar-link {
  color: white;
  text-decoration: none;
  font-size: 18px;
}

.navbar-link:hover {
  color: #ff6347;
}

.footer {
  background-color: rgba(51, 51, 51, 0.5); /* Same transparency as navbar */
  color: white;
  text-align: center;
  padding: 20px 0;
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  z-index: 1000;
}

.footer-text {
  margin: 0;
  font-size: 16px;
}
</style>
