<template>
<b-container>
<div id="rm">
  <form>    <h1>One Rep Max Calculator</h1>
<ul>
  <li>
     <label for="weightLifted">Weight Lifted</label>
    <input type="text" id="weightLifted" v-model="weightLifted">
  </li>
  <li>
     <label for="reps">Number of Reps</label>
    <input type="text" id="reps" v-model="reps">
  </li>
  <li>
       <label for="result">Max</label>
    <input id="result" v-model="result">
  </li>
</ul>
   

  </form></div></b-container>
</template>
<style>
#rm{
  margin: 0 auto;
  widows: 320px;
}
label{
  padding-right: 20px;
  width:140px;
  
}
form{
  color: white;
}
li{
  list-style: none;
}

</style>
<script>

  export default {
  
      name: 'oneRepMax',
     
  data() {
    return {
      weightLifted: '',
      reps: '',
      
    }
  },
  computed:{   
    result: function(){
         return this.weightLifted * (1 + (this.reps / 30));
  }
  }
}
</script>
