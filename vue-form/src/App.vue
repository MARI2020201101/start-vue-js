<template>
<form v-on:submit="submitLogin">
  <div>
    <label for="username">username</label>
    <input type="text"  id="username" v-model="username">
  </div>
  <div>
    <label for="password" >password</label>
    <input type="password" id="password" v-model="password">
  </div>
  <button>Login</button>
</form>
</template>

<script>


export default {
  data:function(){
    return {
      'username':'',
      'password':''
    }
  },
  methods: {
    submitLogin:function(e){
      e.preventDefault();
      console.log(this.username, this.password);
    }
  },
 
}
</script>

<style>

</style>
