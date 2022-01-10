<template>
    <header>
          <img src="../assets/img/spotify-logo.png" alt="Spotify Logo">
    </header>
</template>

<script>
export default {
    name: "Header"
}
</script>

<style scoped lang="scss">
@import '../style/variables';
header{
   background-color: $primary_color;
        img{
            margin: 20px;
            width: 50px;
        }
}
</style>