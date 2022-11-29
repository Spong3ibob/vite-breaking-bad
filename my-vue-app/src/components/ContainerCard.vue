<script>
import axios from "axios"
import AppCard from './AppCard.vue'

export default {
    components: {
        AppCard,

    },
    data(){
        return{
            characters:[]
        }
    },
    created(){
         axios.get("https://www.breakingbadapi.com/api/characters").then((resp) => {
            this.characters = resp.data;
            console.log(resp.data)
         })
    }

}
</script>

<template>
  <div class="container">
    <div class="bar">
        <h3>Found 62 charcters</h3>
    </div>
    <AppCard
    v-for="character in characters"
    :info="character"
    />
  </div>
 
</template>

<style lang="scss" >
.container{
    background-color: var(--secondary-color);
    width: 80%;
    height: 100%;
    margin: auto;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}
.bar{
    height: 50px;
    width: 80%;
    background-color: var(--third-color);
   
    h3{
        display: flex;
        align-items: center;
        color: var(--secondary-color);
    }
}
</style>
