<template>
    <div class="card">
        <img :src="details.poster" alt="">

        <h2>{{details.title}}</h2>

        <h4>{{details.author}}</h4>
        <h4>{{details.year}}</h4>
    </div>
</template>

<script>
export default {
    name:"Card",
    props:{
        details: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
.card{
    width: calc( (100% / 5) - 40px );
    margin: 20px;
    background-color: $primary_color;
    padding: 25px;
    text-align: center;

    h2{
        text-transform: uppercase;
        font-size: 20px;
        margin: 15px 0;
    }
    h4{
        text-transform: uppercase;
        color: grey;
    }
}
</style>