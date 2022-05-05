<template>
    <div>
        <img src="../assets/images/jumbotron.jpg" alt="">
    </div>
    
</template>

<script>
export default {
    name:'AppJumbo',
}
</script>

<style lang="scss" scoped>
@import "../style/variables";
    
    img{
        width: 100%;
        height: 400px;
        object-fit: cover;
        object-position: 100% 0%;
    }
</style>