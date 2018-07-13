<template>

  <b-container fluid>

    <b-navbar class="row" toggleable="lg">


      <b-navbar-brand class="col-sm-3">
        <div id="header">
          <b-link to="/">Carlin Athletics </b-link>
        </div>
      </b-navbar-brand>

      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
      <b-collapse is-nav id="nav_collapse">
        <b-navbar-nav>
          <b-nav-item to="goldenRatio"><h5> Golden Ratio in Bodybuilding </h5></b-nav-item>
          <b-nav-item to="oneRepMax"><h5>One Rep Max Calculator</h5>  </b-nav-item>
          <b-nav-item href="https://www.reddit.com/r/Fitness/wiki/programs"><h5>Training Guides</h5>  </b-nav-item>
          <b-nav-item to="trainingGuides"> <h5>Workout Gear</h5> </b-nav-item>
          <b-nav-item to="trainingGuides"> <h5>Supplements</h5> </b-nav-item>
          <b-nav-item to="posts"><h5>Articles</h5></b-nav-item>
           <b-nav-item to="/FFMI"><h5> FFMI </h5></b-nav-item>


        </b-navbar-nav>
      </b-collapse>

    </b-navbar>
    <div id="banner">
      <h3>Training The Next Generation Of Athletes</h3>

    </div>
  </b-container>
</template>
<script>
  export default {

  }
</script>
<style>
  @import url('https://fonts.googleapis.com/css?family=Acme');
  .navbar {
    background-color: rgb(0, 0, 0);
    margin: 0 auto;
    text-decoration: none;
  }

  a {
    text-decoration: none;
    color: white;
  }

 .nav-link h5  {
    color: white;
  
  }
  #dropDown a {
    color: rgb(255, 255, 255);
    width: 150px;

  }

  .navbar-brand {
    font-size: 3.2em;
    text-align: center;
  }

  .nav-item {
    padding: 1px;
  }

  #header {
    color: rgb(0, 0, 0);
    font-family: 'Acme', sans-serif;
    -webkit-font-smoothing: antialiased;
    

  }
 

  #header {
   
    font-size: .8em;
  display: inline-block;
  }

  #banner {
    background-color: rgba(255, 255, 255, 0.267);
    text-align: right;
  }

  .navbar-toggler {
    width: 100vw;
    margin: 0 auto;
    height: auto;
    background-color: white;
  }

  #banner h3 {
    color: rgb(255, 255, 255);
  }

  @media only screen and (max-width: 740px) {

    #banner h3 {
      text-align: center;
      font-size: 1em;

    }
  }

  @media (max-width: 360px) {

    .navbar {
      font-size: .6em;
    }
  }
   @media only screen and (max-width: 992px) {

    #header {
      text-align: center;
     

    }
  }
</style>