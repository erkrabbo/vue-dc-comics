<template>
  <div class="random">
    <ul>
      <li v-for="(ele, index) in eleList" :key="index">
        <a href="#">
          <img :src="getImgUrl(ele.img)" alt="ele.img">
          <p>{{ ele.text }}</p>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: 'MainContentFooter',
      eleList: [
        {
          img: 'buy-comics-digital-comics.png',
          text: 'DIGITAL COMICS'
        },
        {
          img: 'buy-comics-merchandise.png',
          text: 'DC MERCHANDISE'
        },
        {
          img: 'buy-comics-shop-locator.png',
          text: 'SUBSCRIPTION'
        },
        {
          img: 'buy-comics-subscriptions.png',
          text: 'COMIC SHOP LOCATOR'
        },
        {
          img: 'buy-dc-power-visa.svg',
          text: 'DC POWER VISA'
        }
      ]
    }
  },
  methods: {
    getImgUrl (element) {
      return require('../assets/img/' + element)
    }
  }
}
</script>

<style scoped lang="scss">
  .random{
      background-color: #0282f9;
  }
  ul{
    font-size: 10px;
    list-style: none;
    display: flex;
    margin: 0 auto;
    max-width: 900px;
    padding: 2rem 0;
    li{
        flex-grow: 1;
        display: flex;
        align-items: center;
    }
    a{
        display: flex;
        align-items: center;
        text-decoration: none;
        color: white;
        white-space: nowrap;
    img{
        max-width: 50px;
        max-height: 50px;
        padding: .5em;
    }
    }
  }
</style>
