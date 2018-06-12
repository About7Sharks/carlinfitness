<template>
<b-container>
  <navbar/>
<div id="rm">
  <form>    <h1>One Rep Max Calculator</h1>

    <label for="weightLifted">Weight Lifted</label>
    <input type="text" id="weightLifted" v-model="weightLifted">
    <br/>
    <label for="reps">Number of Reps</label>
    <input type="text" id="reps" v-model="reps">
    <br/>
    <label for="result">Max</label>
    <input id="result" v-model="result">
  </form></div></b-container>
</template>
<style>
#rm{
  margin: 0 auto;
  widows: 320px;
}
label{
  padding-right: 20px;
  
}
form{
  color: white;
}

</style>
<script>
import navbar from '~/components/navbar.vue'

  export default {
    components:{
      navbar
    },
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
