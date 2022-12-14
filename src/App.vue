<script setup>
import { RouterLink, RouterView } from 'vue-router'


import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header class="header">
    
    <div class="header-item">
      <div class="nav-logo">
        <img src="@/assets/images/logo/atelier.png" alt="">
      </div>
    </div>
    <div class="header-item">
      <nav class="nav">
        <RouterLink class="nav-link" to="/">Home</RouterLink>
        <RouterLink class="nav-link" to="/about">About</RouterLink>
        <RouterLink class="nav-link" to="/test">Test</RouterLink>
      </nav>
    </div>
    <div class="header-item">
      <div class="header-logo">
        <img src="./assets/images/logo/step.png" alt="">
      </div>
    </div>

  </header>
  <!-- <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/test">Test</RouterLink>
      </nav>
      
    </div>
  </header> -->

  <RouterView />

  <footer class="footer">
    test
  </footer>
</template>

<style lang="scss" scoped>
@use './styles/variables' as *;

.header {
  position: fixed;
  height: 4rem;
  width: 100%;

  background-color: $bg-nav;
  padding: 0 1rem;
  
  display: flex;
  justify-content: space-between;
  align-items: center;

  &-item {
    overflow: hidden;

    img {
      display: block;
      width: 150px;
    }
  }
}
.nav {
  display: flex;
  align-items: center;

  &-link {
    font-size: $text-lg;
    font-weight: 500;
    margin-right: 1.5rem;

    &:last-child {
      margin-right: 0;
    }
  }
}
</style>
