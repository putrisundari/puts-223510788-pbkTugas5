<template>
    <nav class="navbar">
      <div class="navbar-brand">Sunrise Shop</div>
      <ul class="navbar-nav">
        <li><a href="#">Home</a></li>
        <li><a href="#">Products</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'Navbar'
  }
  </script>
  
  <style scoped>
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #b53f7a;
    padding: 10px 20px;
    color: rgb(227, 165, 189);
  }
  
  .navbar-brand {
    font-size: 1.5rem;
  }
  
  .navbar-nav {
    list-style: none;
    display: flex;
    gap: 15px;
  }
  
  .navbar-nav li a {
    color: white;
    text-decoration: none;
  }
  
  .navbar-nav li a:hover {
    text-decoration: underline;
  }
</style>