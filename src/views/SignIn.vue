<template>
  <div>
    <form @submit.prevent="submit">

      <div>
        <label for="email">Email</label>
        <input type="text" name="email" v-model="form.email">  
      </div>

      <div>
        <label for="password">Password</label>
        <input type="password" name="password" id="password" v-model="form.password">
      </div>

      <div>
        <button type="submit">SignIn</button>
      </div>

    </form>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  name: 'signin',
  components: {
    
  },
  data(){
    return{
      form:{
        email: '',
        password: '',
      }
    }
  },
  methods: {
    async submit(){
      let response = axios.post('auth/signin', this.form)
      console.log(response.data);
    }
  }
}
</script>
