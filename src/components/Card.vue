<template>
    <div class="card">
        <img src="https://cdn2.jazztimes.com/2018/05/SteveGadd-800x723.jpg" alt="">

        <h2>name</h2>

        <h4>autor</h4>
        <h4>year</h4>
    </div>
</template>

<script>
export default {
    name:"Card"
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