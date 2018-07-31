<template>
  <b-container fluid>
    <navbar/>

    <div id="leftFrank" class="col-sm-6">
      <h1>
        Combining the Art and Science of Fitness
      </h1>
      <h3>The Greatest Athletes leave nothing to chance. Their greatness is a result of thier time dedicated to perfecting their
        craft. </h3>
      <br>
    </div>
    <img src="../static/frankZane.jpg" id=Franky alt="">



  </b-container>
</template>

<script>
  export default {

  }
</script>

<style>
  #__layout {
    background-color: black;
  }

  #links a {
    background-color: #313030;
    border: 1px solid white;
  }



  #leftFrank {
    color: white;

    min-width: 375px;

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

  @media (max-width: 360px) {
    .subtitle {
      min-width: 100%;
    }
    #leftFrank {
      min-width: 100%;
    }

  }
</style>