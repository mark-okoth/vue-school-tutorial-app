<template>
  <div id="app">
    <div id="nav">
     <navbar/>
    </div>
    <router-view/>
  </div>
</template>
<script>
import navbar from './components/navbar/navbar'
  export default{
    components:{
    navbar
    },
    data() {
      return {
        
      }
    },
  }
</script>

<style>
*{
  margin: 0;
  padding: 0;
}



</style>
