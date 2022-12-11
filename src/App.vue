<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <!-- <img alt="Vue logo" class="logo" src="@/assets/logo.png" width="125" height="125" /> -->

    <div class="wrapper">
      <!-- <HelloWorld msg="Vectis" /> -->
      <img alt="Vue logo" class="logo imglogo" src="@/assets/novalogo1.png" width="300" height="225"/>
      <nav>
        <RouterLink to="/">Serviços</RouterLink>
        <RouterLink to="/about">sobre</RouterLink>
        <RouterLink to="/contact">Contato</RouterLink>
      </nav>
    </div>
    
  </header>

  <RouterView />
  <p style="margin:10px">copyright © by <a href="https://api.whatsapp.com/send?phone=5582996909200&text=Oi,%20tenho%20interesse%20em%20seus%20servi%C3%A7os%20de%20desenvolvimento"> Dev. Ensinar</a> - 2022</p>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;

    transition: all 0.5s;
    cursor: pointer;
  }

  .logo:houver {
    -webkit-filter: drop-shadow(15px 10px 5px rgba(0,0,0,.5));
    filter: drop-shadow(15px 10px 5px rgba(0,0,0,.5));
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
   
}
</style>
