<template>
  
<b-container>
  <navbar/>
    <br>
<div id="instructionText">
    <h2>Record the following Measurments</h2>
    <p>Unit of Measurments doesn't matter since everything is being calculated off of ratios you could measure your golden porportions
      with dirty socks if you wanted too.
    </p>
</div>
<form>      <li>
        <label for="bicep">Circumfrence of Bicep</label>
        <br>
        <input v-model="bicep">
      </li>
      <li>
        <label for="wrist">Circumfrence of Wrist</label>
        <br>
        <input v-model="wrist">
      </li>
      <li>
        <label for="shoulders">Circumfrence of Shoulders</label>
        <br>
        <input v-model="shoulders">
      </li>
      <li>
        <label for="chest">Circumfrence of Chest</label>
        <br>
        <input v-model="chest">
      </li>
      <li>
        <label for="waist">Circumfrence of Waist</label>
        <br>
        <input v-model="waist">
      </li>
      <li>
        <label for="upperThigh">Circumfrence of Upper Thigh</label>
        <br>
        <input v-model="upperThigh">
      </li>
      <li>
        <label for="knee">Circumfrence of Knee</label>
        <br>
        <input v-model="knee">
      </li>
      <li>
        <label for="calves">Circumfrence of Calves</label>
        <br>
        <input v-model="calves">
      </li>

</form> 

<div id='measurments'>
   <ul>
      <h2>Ideal Measurments</h2>
      <li>
        Arms: {{idealArm}}
      </li>
      <li>
        Calves: {{idealCalves}}
      </li>
      <li>
        Shoulders: {{idealShoulders}}
      </li>
      <li>Chest: {{idealChest}}
      </li>
      <li>Legs: {{idealLegs}}</li>
    </ul>
    <ul>
      <h2>Current Measurments</h2>
      <li>Arms: {{bicep}}</li>
      <li>Calves: {{calves}}</li>
      <li>Shoulders: {{shoulders}}</li>
      <li>Chest: {{chest}}</li>
      <li>Legs: {{upperThigh}}</li>
    </ul>
    <ul >
      <h2>Difference</h2>
      <li>Arms: {{idealArm - bicep}}</li>
      <li>Calves: {{idealCalves - calves}}</li>
      <li>Shoulders: {{idealShoulders - shoulders}}</li>
      <li>Chest: {{idealChest - chest}}</li>
      <li>Legs: {{idealLegs - upperThigh}}</li>
    </ul></div>
  </b-container>

</template>

<script>

  export default {
   
    name: 'goldenRatio',
    data() {
      return {
        bicep: '',
        wrist: '',
        shoulders: '',
        waist: '',
        upperThigh: '',
        knee: '',
        calves: '',
        chest: ''
      }
    },
    computed: {
      //   Your arms when flexed should be 150% bigger than your wrist circumference.
      idealArm: function () {
        return (this.wrist * 2.5)
      },
      idealCalves: function () {
        return (this.bicep)
      },
      idealShoulders: function () {
        return (this.waist * 1.618)
      },
      idealChest: function () {
        return (this.wrist * 6.5)
      },
      idealLegs: function () {
        return (this.knee * 1.75)
      }

    }

  }

</script>

<style>
  li {
    list-style: none;
   
  }

  #instructionText{
      width: 95%;
        min-width: 320px;
        text-align: center;
        padding-bottom: 20px;
                color: white;

  }
form{
    min-width: 320px;
    text-align: center;
    color: white;
    }
    input{
        border: 1px solid #3b8070;

    }
    h2{
        text-align: center;
    }
    #measurments{
        max-width: 320px;
        margin: 0 auto;
        color: white;
    }
   
</style>







// functionality // explanation // style
