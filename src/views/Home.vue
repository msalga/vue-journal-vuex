<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
  <button @click="godaybook()" class="btn btn-primary">es mi boton</button>
    <button class="btn btn-secondary">es mi boton</button>
      <button class="btn btn-success">es mi boton</button>

  </div>
</template>

<script>

export default {
  methods:{
      godaybook(){
        this.$router.push({name:'no-entry'})
      }
  }
}
</script>
