<script>
import AppTitle from './components/AppTitle.vue'
import ContainerCard from './components/ContainerCard.vue'


export default {
  components: {
    AppTitle,
    ContainerCard
  }
}
</script>

<template>
  <AppTitle />
  <select name="category" id="">
    <option value="">Select Category</option>
  </select>
  <ContainerCard/>
</template>

<style>
@import url(../global.scss);
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700&display=swap');
*{
  font-family: 'Roboto', sans-serif;
  background-color: var(--primary-color);
}
select{
  border: none;
  background-color: var(--secondary-color);
  padding: 5px;
  border-radius: 5%;
  margin-left: 300px;
  margin-top: 20px;
  margin-bottom: 15px;
}

</style>
