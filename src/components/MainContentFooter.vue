<template>
  <div class="random">
    <ul>
      <li>
          <a href="#">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <p>DIGITAL COMICS</p>
          </a>
      </li>
      <li>
          <a href="#">
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <p>DC MERCHANDISE</p>
          </a>
      </li>
      <li>
          <a href="#">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <p>SUBSCRIPTION</p>
          </a>
      </li>
      <li>
          <a href="#">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <p>COMIC SHOP LOCATOR</p>
          </a>
      </li>
      <li>
          <a href="#">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <p>DC POWER VISA</p>
          </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: 'MainContentFooter'
    }
  },
  methods: {
    getImgUrl (ele) {
      return '../assets/img/' + ele.imgSrc
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
