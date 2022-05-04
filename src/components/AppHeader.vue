<template>
  <header>
    <img src="../assets/images/dc-logo.png" alt="">
    <nav>
      <ul>
        <li v-for="(item,index) in links" :key="index" :class="{'selected' : item.active}">
          {{item.testo}}
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'AppHeader',
  data(){
    return{
      links: [
        {
          testo: "Characters",
          link: "",
          active: false,
        },
        {
          testo: "Comics",
          link: "",
          active: true,
        },
        {
          testo: "Movies",
          link: "",
          active: false,
        },
        {
          testo: "Tv",
          link: "",
          active: false,
        },
        {
          testo: "Games",
          link: "",
          active: false,
        },
        {
          testo: "Collectibles",
          link: "",
          active: false,
        },
        {
          testo: "Videos",
          link: "",
          active: false,
        },
        {
          testo: "Fans",
          link: "",
          active: false,
        },
        {
          testo: "News",
          link: "",
          active: false,
        },
        {
          testo: "Shop",
          link: "",
          active: false,
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import "../style/variables";

  .selected{
    color: $dcblue;
  }
  header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: $dcwhite;
    width: $dcwidth;
    margin: auto;
  }
  nav ul {
    display: flex;
    margin-left: 20px;
    list-style-type: none;
    gap: 30px;
    cursor: pointer;
    padding: 40px;
    text-transform: uppercase;

  }
  nav ul li{
    font-size: $dcsize;
  }
  img{
    width: 60px;
  }
  

</style>
