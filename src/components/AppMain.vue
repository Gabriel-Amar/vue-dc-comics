<template>
    <main>
        <ul>
            <li v-for="(item, index) in links" :key="index">
                <img :src="item.img" alt="">
                {{item.testo}}
            </li>
        </ul>
    </main>
</template>

<script>
export default {
    name: 'AppMain',
    data(){
        return{
            links: [
                {
                    testo: "Digital Comics",
                    img: require("../assets/images/buy-comics-digital-comics.png"),
                },
                {
                    testo: "Dc Merchandise",
                    img: require("../assets/images/buy-comics-merchandise.png"),
                },
                {
                    testo: "Subscription",
                    img: require("../assets/images/buy-comics-subscriptions.png"),
                },
                {
                    testo: "Comic shop locator",
                    img: require("../assets/images/buy-comics-shop-locator.png"),
                },
                {
                    testo: "Dc power visa",
                    img: require("../assets/images/buy-dc-power-visa.svg"),
                },
            ]
        }
    }

}
</script>

<style scoped lang="scss">
    @import "../style/variables";
    main{
        background-color: $dcblue;
        
    }
    ul{
        display: flex;
        justify-content: space-between;
        width: $dcwidth;
        margin: auto;
        padding: 50px;
        cursor: pointer;
    }
    li{
        display: flex;
        align-items: center;
        gap: 10px;
        color: $dcwhite;
    }
    img{
        width: 45px;
    }

</style>
