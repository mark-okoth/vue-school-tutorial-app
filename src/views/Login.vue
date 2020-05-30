<template>
    <div class="login">
        <div class="login-container">
            
            <form @submit.prevent="onSubmit" class="inputs" >
                <h2>Login now</h2>
                <div class="input-field">
                    <input type="email" v-model="email" placeholder="Please Enter An Email">
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
export default {
     
    data(){
        return{
          email:"",
          password: ""
        }
    }
}
</script>

<style>
.login{
    background:  rgba(27, 2, 85, 0.767);
    width: 100vw;
    height: 100vh;
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
</style>