<template>
   <h1 v-if="show">Hii This is Ajay speaking</h1>
   <h2 v-else>Ajay is out of the station</h2>
   <button @click="toggle()">Toggle button</button>
</template>

<script>

export default{
  name: "Login-form",
  data() {
    return{
       show: true
    }
  },
method: {
   toggle() {
    this.show = !this.show
   }
}
}
</script>

<style scoped>
h1 {
    font-family: 'Courier New', Courier, monospace;
}
h2 {
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}
</style>