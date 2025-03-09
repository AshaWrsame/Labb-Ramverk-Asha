<script>
export default {
  name:'FooterComp'
}
</script>
<template>
  <footer class="footer">
    <div class="container">
      <p class="footer-text">© 2025 FEU ITHS. All rights reserved.</p>
    </div>
  </footer>
</template>


<style>
.footer {
  background-color: rgba(51, 51, 51, 0.5);
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
