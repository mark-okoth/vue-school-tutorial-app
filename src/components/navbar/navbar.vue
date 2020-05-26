<template>
    <div class="navbar">
    <nav>
      <div class="nav-container">
         <ul>
           <li><a href="">Home</a></li>
           <li><router-link to="/about">About</router-link></li>
           <li><a href="">Topics</a></li>
           <li><a href="">Paths</a></li>
           <li><a href="">Login</a></li>
         </ul>
         

      </div>
    </nav>
        
    </div>
</template>
<script>
  export default {
    name: 'navbar',
    components: {},
    data() {
      return {
        
      }
    },
    computed: {},
    mounted() {
    },
    methods: {}
  }
      
  </script>

  <style scoped>

  nav{
    width: 20vw;
    background: black;
    height: 100vh;
  }
  .nav-container{
    display: flex;
    justify-content: center;
    align-items: center;
    align-content: center;
  }

  ul{
    margin: 80px 0 ;
    list-style: none;
  }
  ul li{
    padding: 20px;
  }

  ul li a{
    text-decoration: none;
    font-size: 1.3rem;
    
  }
  
  </style>