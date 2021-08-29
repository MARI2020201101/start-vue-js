<template>
  <div>
      <h1>header</h1>
      {{ propsData }}
      <button v-on:click="sendData">send</button>
  </div>
</template>

<script>
  export default{
    props:['propsData'],
    methods: {
       sendData:function(){
            this.$emit('renew')
        }
    }
  }
</script>

<style>

</style>
