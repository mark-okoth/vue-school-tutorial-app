<template>
  <div id="app">
    <navbar />
    <router-view />
  </div>
</template>
<script>
import navbar from "./components/navbar/navbar";
export default {
  components: {
    navbar
  },
  data() {
    return {
      
    };
  }
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  display: flex;
  height: 100vh;
  flex-direction: row;
}
</style>
