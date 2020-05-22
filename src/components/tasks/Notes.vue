<template>
  <div class="Notes">
    <div class="container">
      <form @submit.prevent="adding">
        <input type="text" v-model="posttitle" placeholder="enter the note below" />
        <p v-if="feedback" class="feedback">{{feedback}}</p>
        <input
          type="text"
          v-model="notes"
          @keydown.enter="adding"
          placeholder="type the notes here"
        />
        <p v-if="feedback" class="feedback">{{feedback}}</p>
        <button class="post">Add</button>
      </form>
      <div class="note-container pipes" v-for="(detail, index) in details" :key="index">
        <h3>{{title}}</h3>
        <p>{{detail}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      posttitle: null,
      title: '',
      notes: null,
      details: [],
      feedback: null
    };
  },
  methods: {
    adding() {
      if (this.notes) {
        this.details.push(this.notes);
        this.notes = null;
        this.feedback = null;
      } else {
        this.feedback = "You Must Enter A Note";
      }
      if(this.posttitle){
          this.title = this.posttitle
          this.feedback = null
          this.posttitle =null
      }else{
          this.feedback = 'You must enter a title'
      }
    }
  }
};
</script>

<style scoped>
.container {
  width: 33.3vw;
  border: 1px solid white;
  height: 100vh;
  border: none;
  display: flex;
  flex-direction: column;
}
form {
  display: flex;
  flex-direction: column;
  margin: 20px auto;
}
input {
  width: 300px;
  padding: 10px;
  margin: 10px 0;
  outline: none;
  color: white;
  background: hsl(207, 26%, 17%);
  border-top: none;
  border-right: none;
  border-left: none;
  border-bottom: 1px solid white;
}
::placeholder {
  color: white;
  text-transform: capitalize;
}
button {
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  background: rgb(46, 81, 94);
  padding: 10px;
  outline: none;
}

.note-container {
  width: 400px;
  text-align: center;
  margin: 0 auto;
}
.feedback {
  color: red;
  font-style: italic;
  font-weight: lighter;
}
</style>