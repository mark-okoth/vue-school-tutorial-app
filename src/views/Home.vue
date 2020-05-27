<template>
  <div class="home">
    <div class="home-container">
     
     <p>Learn to code for free with curated video tutorials!</p>
     <a href="">CREATE AN ACCOUNT</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {}
};
</script>
<style>
.home {
  background-image: url("../assets/pic.jpeg");
  background-color: rgb(28, 28, 95);
  background-blend-mode: multiply;
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
}

.home-container{
  margin: 20px 20vw;
}
.home-container p{
  font-size: 3.5rem;
  margin-bottom: 20px;
}
.home-container a{
  text-decoration: none;
  background:lightslategray;
  padding: 15px 20px;
}

.home-container a:hover{
  background: white;
  border: ipx solid lightslategrey;
  color: slateblue;
}
</style>