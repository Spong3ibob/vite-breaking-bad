<script>
export default {
  data() {
    return {
      title:"Breaking Bead Api"
    }
  }
}
</script>

<template>
  <div class="title">
    <img src="../assets/logo.png" alt=""> 
    <h1>{{title}}</h1>
  </div>
 
</template>

<style scoped>
.title{
  display: flex;
  padding: 10px;
}
img{
  height: 35px;
}
h1{
  color: var(--secondary-color);
}
</style>
