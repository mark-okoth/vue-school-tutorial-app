<template>
    <div class="login">
        <div class="login-container">
            
            <form @submit.prevent="onSubmit" class="inputs" >
                <h2>Login now</h2>
                <div class="input-field" >
                    <input 
                        type="email" 
                        :class="{invalid: $v.email.$error}"
                        v-model="email" @input="$v.email.$touch()" 
                        placeholder="Please Enter An Email"
                        >
                    <!-- <p>{{$v}}</p> -->
                </div>
                   <div class="input-field" >
                    <input type="passoword" v-model="password" placeholder="Please Enter a password">
                </div>
                <button type="submit">Login</button>
            </form>
        </div>
    </div>
</template>

<script>
import {required, email} from "vuelidate/lib/validators";
export default {
     
    data(){
        return{
          email:"",
          password: ""
        }
    
    },
    validations:{
      email:{
          required,
          email
      }
    }
}
</script>

<style>
.login{
    background:  rgba(27, 2, 85, 0.767);
    width: 100vw;
    height: 101vh;
}
.inputs{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
}

input{
    width: 20vw;
    padding: 10px;
    margin: 10px;
    outline: none;
    border: 2px solid white;
    color:white;
    border-top:none ;
    border-right:none;
    border-left: none;
    background: inherit
}
::placeholder{
    font-size: 1.1rem;
    color: white;
}
button{
width: 22vw;
padding: 10px;
color:black;
background: white
}
h2{
    text-align: center;
    margin: 30px auto;
}
.invalid{
    border-bottom: 2px solid red;
}
</style>