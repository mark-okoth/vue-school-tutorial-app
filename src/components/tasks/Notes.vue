<template>
    <div class="Notes">
        <div class="container">
           <form @submit.prevent="send">
              <input type="text" v-model="posttitle" placeholder="enter the note below"> 
              <input type="text" v-model="notes" @keydown.tab="adding" placeholder="type the notes here">
              <p v-if="feedback" class="feedback">{{feedback}}</p>
               <button class="post">Add</button>
               </form> 
             <div class="note-container">
                 <h3>{{posttitle}} </h3>
                 <p>{{notes}}</p>
             </div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
          posttitle: null,
          notes:null,
          details:[ ],
          feedback:null
        }
    },
    methods:{
        send(){
          console.log
        },
         adding(){
             if(this.notes){
              this.details.push(this.notes)
              console.log(this.details)
              this.notes = null
              this.feedback = null
             }else{
                 this.feedback = "You Must Enter A Value"
                
             }
         }
    },
   
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
    background: rgb(46, 81, 94);
    padding: 10px;
    outline: none;
    
}

.note-container{
    width: 400px;
    text-align: center;
    margin: 0 auto;
    
}
h3{
    font-style: italic;
    font-weight: 100;
}
.feedback{
    color: red;
    font-style: italic;
    font-weight: lighter;
}

</style>