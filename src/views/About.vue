<template>
  <div class="about">
    <h3>the About page</h3>
    <p>this is a content management app for planning from planning tasks job and connecting with friends v1.0.0</p>
  </div>
</template>

<script>
export default {
  name:"about",
  data(){
    return{

    }
  }
}
</script>

<style scoped>
.about{
  width: 60vw;
  display: flex;
  height: 80vh;
  flex-direction: column;
  margin:  0 auto;
  align-items: center;
  justify-content: center;
}
h3{
  text-align: center;
  margin: 2em auto;
}
</style>