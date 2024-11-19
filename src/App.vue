import AboutView from '@/views/AboutView.vue';
<script setup>

</script>
<template>
  <nav>
    <ul>
      <li>
        <RouterLink class="rout" to="/">Home</RouterLink>
      </li>
      <li>
        <RouterLink class="rout" to="/about">About</RouterLink>
      </li>
      <li>
        <RouterLink class="rout" to="/contact">Contact</RouterLink>
      </li>
      <li>
        <RouterLink class="rout" to="/productlist">Product List</RouterLink>
      </li>
    </ul>
  </nav>
  <main>
    <RouterView />
  </main>
</template>

<style>
  nav {
    background-color: rgb(133, 118, 95);
    color: white;
    padding: 5%;
    text-align: center;
  }

  nav ul, ul {
    list-style-type: none;
    margin: 3px;
    padding: 0;
    display: flex;
  }

  nav a {
    
    margin-left: 5px;
    margin-right: 5px;
    color: white;
    font-weight: bold;
    font-size: larger;
  }

  main a {
    color: rgb(223, 255, 82);
    background-color: black;
    padding: 3px;
    border-radius: 5px;
  }

  li {
    margin: 5px;
  }
</style>