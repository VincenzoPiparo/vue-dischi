<template>
    <main>
        <div class="container">
            <div class="list_card">
                <Card v-for="(disc, index) in listCard" :key="index" :details="disc"/>
            </div>
        </div>
    </main>
</template>

<script>
import Card from "./Card.vue"
import axios from 'axios';

export default {
    name: "Main",
        components:{
            Card
        },
        data: function(){
            return{
                listCard: []
            };
        },
        methods: {
            getMusic: function () {
                axios.get('https://flynn.boolean.careers/exercises/api/array/music')
                .then((response) => {
                    this.listCard = response.data.response;
                });
            }
        },
        created: function(){
            this.getMusic();
        }
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