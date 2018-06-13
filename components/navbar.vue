<template>

  <b-container fluid>

    <b-navbar class="row" toggleable="lg">


      <b-navbar-brand class="col-sm-6">
        <div id="header">
          <b-link to="/">Carlin Athletics </b-link>
        </div>
      </b-navbar-brand>

      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
      <b-collapse is-nav id="nav_collapse">
        <b-navbar-nav>
          <b-nav-item to="goldenRatio">Golden Ratio in Bodybuilding </b-nav-item>
          <b-nav-item to="oneRepMax">One Rep Max Calculator </b-nav-item>
          <b-nav-item href="https://www.reddit.com/r/Fitness/wiki/programs">Training Guides </b-nav-item>
          <b-nav-item to="trainingGuides">Workout Gear </b-nav-item>
          <b-nav-item to="trainingGuides">Supplements </b-nav-item>
          <b-nav-item to="posts">Articles </b-nav-item>


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
    padding-left: 10px;
  }

  .nav-link {
    font-size: 2em;
    border-radius: 10px;
  }

  #dropDown a {
    color: black;
    width: 150px;

  }

  .navbar-brand {
    font-size: 3.5em;

  }

  .nav-item {
    padding: 15px;
  }

  #header {
    color: rgb(0, 0, 0);
    font-family: 'Acme', sans-serif;
    -webkit-font-smoothing: antialiased;

  }

  #header {
    color: black;
    font-size: 1.3em;
    display: flex;
  }

  #banner {
    background-color: rgba(255, 255, 255, 0.267);
    text-align: right;
  }

  .navbar-toggler {
    width: 100%;
    height: 20px;
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
      text-align: left;
    }
  }
</style>