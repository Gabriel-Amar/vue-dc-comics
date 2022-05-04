<template>
    <div class="bg">
        <footer>
            <button>Sign-Up now!</button>
            <nav>
                <ul>
                    <li v-for="(item, index) in links" :key="index">
                        {{item.testo}}
                        <img :src="item.img" alt="">
                    </li>
                </ul>
            </nav>
        </footer>
    </div>
</template>

<script>
export default {
    name: 'AppFooter',
    data(){
        return{
            links: [
                {
                    testo: "Follow us",
                },
                {
                    img: require("../assets/images/footer-facebook.png"),
                },
                {
                    img: require("../assets/images/footer-twitter.png"),
                },
                {
                    img: require("../assets/images/footer-youtube.png"),
                },
                {
                    img: require("../assets/images/footer-periscope.png"),
                },
                {
                    img: require("../assets/images/footer-pinterest.png"),
                },

            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import "../style/variables";
.bg{
    background-color: $dcfootcolor;
}
footer{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: $dcwidth;
    margin: auto;
    
}
nav ul{
    display: flex;
    list-style-type: none;
    padding: 40px;
    align-items: center;
}
nav ul li {
    font-size: $dcsize;
    color: $dcblue;
    font-weight: bold;
    cursor: pointer;
    text-transform: uppercase;
}
img{
    width: 20px;
}
button{
    cursor: pointer;
    color: $dcwhite;
    text-transform: uppercase;
    border: 2px solid $dcblue;
    padding: 10px;
    background-color: $dcfootcolor;
}
img{
    padding-left: 10px;
    width: 40px;
}
</style>
