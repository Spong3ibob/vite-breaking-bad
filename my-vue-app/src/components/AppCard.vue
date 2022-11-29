<script>
export default {
    props:{
        info: Object,
    }

}
</script>

<template>
    <div class="card">
        <img :src="info.img" alt="">
        <h4>{{info.name}}</h4>
        <span>{{info.category}}</span>
        <span>{{info.status}}</span>
    </div>
 
</template>

<style lang="scss">
.card{
height: 450px;
width: 224px;
background-color: var(--primary-color);
margin: 20px;
display: flex;
justify-content: center;
flex-direction: column;
    img{
        width: 200px;
        margin: 12px;
    }
    h4{
        text-align: center;
        padding: 10px;
        color: var(--secondary-color);
    }
    span{
        text-align: center;
        color: #7e756d;
    }
}

</style>
