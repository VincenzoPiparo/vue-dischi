<template>
    <main>
        <div class="container">
            <div class="list_card">
                <Card />
                <Card />
                <Card />
                <Card />
            </div>
        </div>
    </main>
</template>

<script>
import Card from "./Card.vue"

export default {
    name: "Main",
        components:{
            Card
        },
}
</script>

<style scoped lang="scss">
@import '../style/variables';
main{
    padding: 15px 0;
    height: calc(100% - 70px);
    color: white;
    background-color: $secondary_color;
    .list_card{
        display: flex;
        flex-wrap: wrap;
    }
}
</style>