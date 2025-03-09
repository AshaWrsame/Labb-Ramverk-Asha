<script>
export default {
  name:'NavBar',
  props:{
    currentPage: {
      type: String,
      required: true
    }
  }
}
</script>
<template>
   <nav class="navbar">
    <div class="container">
      <ul class="navbar-list">
        <li class="navbar-item">
          <router-link to="/" class="navbar-link" :class="{active: currentPage === 'home'}" >Home</router-link>
        </li>
        <li class="navbar-item">
          <router-link to="/about" class="navbar-link" :class="{active: currentPage === 'about'}">About</router-link>
        </li>
      </ul>
    </div>
  </nav>
  </template>
  <style scoped>
  .navbar {
    background-color: rgba(51, 51, 51, 0.5);
    padding: 10px 0;
    position: fixed;
    width: 100%;
    z-index: 1000;
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
    color:  grey;
  }
  .navbar-link.active {
    background-color: rgba(51, 51, 51, 0.7);;
    }
</style>
