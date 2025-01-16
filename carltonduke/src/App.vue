<script setup>
import { RouterLink, RouterView } from 'vue-router'
import BabylonScene from './components/BabylonScene.vue'
import LinkButton from './components/LinkButton.vue';
import AboutButton from './components/AboutButton.vue';
import NameLogo from './components/NameLogo.vue';

</script>

<template>
  <header class="bkg-main">
    <div class="back">
      <!---<h1 class="logo">Carlton</h1>
      <h1 class="logo2">Duke</h1>--->
      
      <div class="link-area">
        
      </div>
    </div>
    <NameLogo></NameLogo>
  </header>
  <BabylonScene/>
  <!---<RouterView />-->
</template>

<style scoped>
.bkg-main {
  background-color: rgb(33,33,33);
}

header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  text-transform: uppercase;
  color: #4CAF50;
  font-family: Arial, Helvetica, sans-serif;
  letter-spacing: 3px;
  font-size:5rem;
  margin: 0.1rem 0;
}

.logo2 {
  text-transform: uppercase;
  color: #474747;
  font-family: Arial, Helvetica, sans-serif;
  letter-spacing: 3px;
  font-size:4rem;
  margin: 0.1rem 0;
}

.back {
  padding: 10px;
	justify-content: right;
  align-items: right;
  border-right: 1px solid var(--color-border);
}

.link-area {
  display:flex;
  margin: 5px;
}

.link-button {
  margin: 10px;
  padding: 5px;
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


