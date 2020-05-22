<template>
    <div class="Notes">
        <div class="container">
           <form @submit.prevent="send">
              <input type="text" v-model="posttitle" placeholder="enter the note below"> 
              <input type="text" v-model="notes" placeholder="type the notes here">
               <button class="post">Add</button>
               </form> 
             <div class="note-coontainer">
                 <h3>{{posttitle}}</h3>
                 <p>{{notes}}</p>
             </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
          posttitle: '',
          notes:''
        }
    }
}
</script>

<style scoped>

.container{
    width: 33.3vw;
    border: 1px solid white;
    height: 100vh;
    border: none;
    display: flex;
    flex-direction:column;
}
form{
    display: flex;
    flex-direction: column;
    margin: 20px auto;
    
}
input{
    width: 300px;
    padding: 10px;
    margin: 10px 0;
    outline: none;
    color:white;
    background: hsl(207, 26%, 17%);
    border-top:none;
    border-right:none;
    border-left:none;
    border-bottom: 1px solid white;
}
::placeholder{
    color: white;
    text-transform: capitalize;
}
button{
    display: flex;
    align-items: center;
    justify-content: center;
    color:white;
    background: lightblue;
    padding: 10px;
    outline: none;
}

</style>