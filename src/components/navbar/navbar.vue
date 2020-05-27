<template>
    <div class="navbar">
    <nav>
      <div class="nav-container">
         <ul>
           <li><i class="fas fa-home"></i><router-link to="/">Home</router-link></li>
           <li><i class="fas fa-user"></i><router-link to="/about">About</router-link></li>
           <li><i class="fas fa-laptop-code"></i><a href="">Topics</a></li>
           <li><i class="fas fa-book"></i><a href="">Paths</a></li>
           <li><i class="fas fa-sign-in-alt"></i><a href="">Login</a></li>
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

  i{
    margin: 0 10px;
    font-size: 1.2rem;
    text-align: left;
    color: rgb(145, 145, 241);
   
  }
  
  </style>