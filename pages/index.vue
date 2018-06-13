<template>
  <b-container fluid>
    <navbar/>
    <div class="row">
      <div class="col-sm-6">
        <h2 class="subtitle">
          The Art and Science of Fitness
          <br>
        </h2>

      </div>
      <div id="leftFrank" class="row">
        <h3 class="col-sm-6">The Greatest Athletes leave nothing to chance. Their greatness is a result of thier time dedicated to perfecting their craft.  </h3>
        <br>
     
  </div>
      <img src="../static/frankZane.jpg" id=Franky class="col-sm-6" alt="">
    </div>


  </b-container>
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
    background-color: black;
    min-height: 100vh;
    text-align: center;
    margin: 0 auto;
    max-width: 1500px;

  }
  #links a{
    background-color: #313030;
    border: 1px solid white;
  }


  .title {
    font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    /* 1 */
    font-weight: 300;
    font-size: 100px;
    color: #ffffff;
    letter-spacing: 1px;
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #ffffff;
    word-spacing: 5px;
    padding-bottom: 15px;
    padding-top: 15px;
    width: 50%;
    min-width: 375px;
  }

  .links {
    padding-top: 15px;
  }

  #leftFrank {
    color: white;
    width: 50%;
    min-width: 375px;
    display: flex;
  }

  #Franky {
    padding-left: 40vw;
    min-width: 320px;
    max-width: 80vw;
    width: 100%;
    border-bottom: 2px solid white;
  

  }

  .subtitle a {
    text-decoration: none;
  }

  @media (max-width: 700px) {
    h1.title {
      font-size: 5em;

    }
    #Franky {
      max-width: 100vw;
      padding-left: 35vw;
    }
  }
  @media (max-width: 360px){
    .subtitle{
      min-width: 100%;
    }
    #leftFrank{
      min-width: 100%;
    }
 
  }
</style>