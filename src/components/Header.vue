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
        width: 50px;
        margin: 20px;
    }
}
</style>