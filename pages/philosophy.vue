<template>

    <div id="philosophy">
      <navbar/> <p>
      If your anything like me you may have fallen victum of just blinley going to the gym and going through the motions. With
      out tracking progress. Well this Website is here for Both you and I to stop guessing what we are doing and to start
      approaching fitness from a scientific and creative persuit.
   </p> </div>
</template>

<script>


import navbar from '~/components/navbar.vue'

  export default {
    components: {
      navbar
    }
  }
</script>
<style>
  #philosophy p{
    padding-top: 15px;
    color: white;
    max-width: 800px;
    margin: 0 auto;
    font-size: 1.68em;
  }
</style>
