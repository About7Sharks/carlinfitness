<template>
  <div>
    <navbar/>
    <nuxt/>
  </div>
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

html {
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  text-shadow: 1px 1px 1px rgb(73, 73, 73);
  box-shadow: 0 10px 6px 6px -6px #777;
  background-color: black;
  color: white;
}
#__nuxt{
  background-color: Black;
}
li{
  list-style-type: none;
}
</style>
