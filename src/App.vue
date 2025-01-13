<script setup>

import trueVibeLogo from './assets/truevibe-logo.jpg'
import truevibe1 from './assets/truevibe-1.PNG'
import truevibe2 from './assets/truevibe-2.PNG'
import truevibe3 from './assets/truevibe-3.PNG'
import truevibe4 from './assets/truevibe-4.PNG'
import truevibe5 from './assets/truevibe-5.PNG'
import truevibe6 from './assets/truevibe-6.PNG'


import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import MarkedDown from './components/MarkedDown.vue'

</script>

<template>
<header>

  <div class="wrapper">
  <img class="logo" :src="trueVibeLogo" alt="TrueVibe Logo" />
</div>
</header>

<MarkedDown />
<header>
  <div class="wrapper">
<img :src="truevibe1" alt="TrueVibe Screenshot" />
<img :src="truevibe2" alt="TrueVibe Screenshot" />
<img :src="truevibe3" alt="TrueVibe Screenshot" />
<img :src="truevibe4" alt="TrueVibe Screenshot" />
<img :src="truevibe5" alt="TrueVibe Screenshot" />
<img :src="truevibe6" alt="TrueVibe Screenshot" />

</div>
</header>

<footer>
<h6>Developed by <a href="https://salesscriptlab.com">Cliffton Kaewkarn</a> Check his code out</h6>

</footer>

</template>

<style scoped>


header .wrapper {

  display: flex;
  
  overflow-x: scroll;
  justify-content: center;
  border-radius: 0.5rem;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}


@media (min-width: 1024px) {


  .logo {
    margin: 4rem 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
  footer {
   margin-top: 5rem; 
  }
}
</style>
