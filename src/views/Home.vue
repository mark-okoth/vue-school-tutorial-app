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
  height: 101vh;
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
  background:rgb(28, 28, 95);
  padding: 15px 20px;
  transition: all 500ms ease-in-out;
}

.home-container a:hover{
  background: white;
  border: ipx solid lightslategrey;
  color: slateblue;
}
</style>