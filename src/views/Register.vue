<template>
  <div class="register">
    <div class="register-container">
      <form @submit.prevent="onSubmit" class="inputs">
        <h2>register now</h2>
        <div class="input-field">
          <input
            type="text"
            :class="{invalid: $v.email.$error}"
            v-model="name"
            @input="$v.email.$touch()"
            placeholder="Please Enter Your Name"
          />
          <p v-if="$v.email.$error">Enter a valid email address</p>
        </div>
        <div class="input-field">
          <input
            type="email"
            :class="{invalid: $v.email.$error}"
            v-model="email"
            @input="$v.email.$touch()"
            placeholder="Please Enter An Email"
          />
          <p v-if="$v.email.$error">Enter a valid email address</p>
        </div>
        <div class="input-field">
          <input
            type="password"
            :class="{invalid: $v.password.$error}"
            @blur="$v.password.$touch()"
            v-model="password"
            placeholder="Please Enter a password"
          />
          <p v-if="$v.password.$error">Enter a valid password</p>
        </div>
        <div class="input-field">
          <input
            type="password"
            :class="{invalid: $v.password.$error}"
            @blur="$v.password.$touch()"
            v-model="confirmPassword"
            placeholder="Please Enter a Confirm password"
          />
          <p v-if="$v.password.$error">Enter a valid password</p>
        </div>
        <button type="submit">Register</button>
      </form>
    </div>
  </div>
</template>

<script>
import { required, email, minLength } from "vuelidate/lib/validators";
export default {
  data() {
    return {
      name: "",
      email: "",
      password: "",
      confirmPassword: ""
    };
  },
  validations: {
    email: {
      required,
      email
    },
    password: {
      required,
      minlen: minLength(6)
    }
  }
};
</script>

<style scoped>
.register {
  background: rgba(27, 2, 85, 0.767);
  width: 100vw;
  height: 101vh;
}
.inputs {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

input {
  width: 20vw;
  padding: 10px;
  margin: 10px;
  outline: none;
  border: 2px solid white;
  color: white;
  border-top: none;
  border-right: none;
  border-left: none;
  background: inherit;
}
::placeholder {
  font-size: 1.1rem;
  color: white;
}
button {
  width: 22vw;
  padding: 10px;
  color: black;
  background: white;
}
h2 {
  text-align: center;
  margin: 30px auto;
}
.invalid {
  border-bottom: 2px solid red;
}
p {
  color: red;
  margin-left: 10px;
  font-family: roboto;
}
</style>