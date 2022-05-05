<template>
    <footer>
        <div class="width">
        <section>
            <h2>DC comics</h2>
            <ul>
                <li v-for="(item, index) in links1" :key="index">
                    {{item.testo}}
                </li>
            </ul>
            <h2>Shop</h2>
            <ul>
                <li>
                    Shop DC
                </li>
                <li>
                    Shop DC Collectibles
                </li>
            </ul>
        </section>

        <section>
            <h2>DC</h2>
            <ul>
                <li v-for="(item, index) in links2" :key="index">
                    {{item.testo}}
                </li>
            </ul>
        </section>

        <section>
            <h2>Sites</h2>
            <ul>
                <li v-for="(item, index) in links3" :key="index">
                    {{item.testo}}
                </li>
            </ul>
        </section>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'AppLinks',
    data(){
        return{
            links1:[
                {
                    testo: "Characters",
                },
                {
                    testo: "Comics",
                },
                {
                    testo: "Movies",
                },
                {
                    testo: "TV",
                },
                {
                    testo: "Games",
                },
                {
                    testo: "Videos",
                },
                {
                    testo: "News",
                },
            ],
            links2:[
                {
                    testo: "Terms Of Use",
                },
                {
                    testo: "Privacy policy (New)",
                },
                {
                    testo: "Ad Choises",
                },
                {
                    testo: "Advertising",
                },
                {
                    testo: "Jobs",
                },
                {
                    testo: "Suscriptions",
                },
                {
                    testo: "Talent Workshops",
                },
                {
                    testo: "CPSC Certificates",
                },
                {
                    testo: "Ratings",
                },
                {
                    testo: "Shop Help",
                },
                {
                    testo: "Contact Us",
                },
            ],
            links3:[
                {
                    testo: "DC"
                },
                {
                    testo: "MAD Magazine"
                },
                {
                    testo: "DC Kids"
                },
                {
                    testo: "DC Universe"
                },
                {
                    testo: "DC Power Visa"
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import "../style/variables";
    footer{
        background-image: url(../assets/images/footer-bg.jpg);
        background-repeat: no-repeat;
        height: 430px;
        background-position: center;
        background-size: cover;
        
    section{
        float: left;
        margin-right: 60px;
        margin-top: 60px;
    }
    }
    .width{
        width: 60%;
        margin: auto;
        background-image: url(../assets/images/dc-logo-bg.png);
        height: 100%;
        background-position: right;
        background-repeat: no-repeat;
    }
    ul li {
        cursor: pointer;
        color: gray;
        margin-bottom: 7px;
    }
    h2{
        font-weight: bold;
        color: $dcwhite;
        margin-bottom: 20px;
    }
    
</style>
