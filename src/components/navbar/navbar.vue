<template>
    <div class="navbar">
    <nav>
      <div class="nav-container">
         <ul>
           <li><router-link to="/"><i class="fas fa-home"></i>Home</router-link></li>
           <li><router-link to="/about"><i class="fas fa-user"></i>About</router-link></li>
           <li><router-link to=""><i class="fas fa-laptop-code"></i>Topics</router-link></li>
           <li><router-link to=""><i class="fas fa-book"></i> Path</router-link></li>
           <li><router-link to=""><i class="fas fa-sign-in-alt"></i>Login</router-link></li>
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
    background:rgb(28, 28, 95);
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
    margin: 0 15px;
    font-size: 1.2rem;
    text-align: left;
    color: white;
   
  }
  
  </style>