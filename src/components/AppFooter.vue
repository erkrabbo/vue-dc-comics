<template>
  <div>
    <div class="container">
      <ul>
          <ul v-for="(list, index) in footerLists" :key="index">
              <h3>{{list.title}}</h3>
              <li v-for="(section, index) in list.sections" :key="index + 1"><a href="#">{{ section }}</a></li>
          </ul>
      </ul>
    </div>
    <div class="footer-footer">
      <div class="cont">
        <a>SIGN-UP NOW!</a>
        <div class="social">
          <span>FOLLOW US</span>
          <img src="../assets/img/footer-facebook.png" alt="">
          <img src="../assets/img/footer-twitter.png" alt="">
          <img src="../assets/img/footer-youtube.png" alt="">
          <img src="../assets/img/footer-pinterest.png" alt="">
          <img src="../assets/img/footer-periscope.png" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: 'AppFooter',
      footerLists: [
        {
          title: 'DC COMICS',
          sections: [
            'Characters',
            'Comics',
            'Movies',
            'TV',
            'Games',
            'Videos',
            'News'
          ]
        },
        {
          title: 'SHOP',
          sections: [
            'Shop DC',
            'Shop DC Collectibles'
          ]
        },
        {
          title: 'DC',
          sections: [
            'Terms Of Use',
            'Privacy policy (New)',
            'Ad Choices',
            'Advertising',
            'Jobs',
            'Subscriptions',
            'Talent Workshops',
            'CPSC Certificates',
            'Ratings',
            'Shop Help',
            'Contact Us'
          ]
        },
        {
          title: 'SITES',
          sections: [
            'DC',
            'MAD Magazine',
            'DC Kids',
            'DC Universe',
            'DC Power Visa'
          ]
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
div{
  background: url('../assets/img/footer-bg.jpg');
  max-height: 350px;
  .container{
    background: right/50% no-repeat url('../assets/img/dc-logo-bg.png');
    padding: 2em;
  }
}
ul{
  list-style: none;
  max-height: 300px;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  align-content: flex-start;
  margin-right: 1em;
  h3{
    color: white;
    margin: .3em 0;
  }
  a{
    text-decoration: none;
    color: grey;
  }
}
.footer-footer{
  padding: 1em 0;
  background: rgb(53, 52, 52);
  // justify-content: space-between;
  a{
    display: flex;
    align-items: center;
    padding: .5em;
    color: white;
    border: 1px solid blue;
  }
  div{
    background: rgb(53, 52, 52);
  }
  .cont{
    background: rgb(53, 52, 52);
    justify-content: space-between;
    display: flex;
    white-space: nowrap;
    align-items: center;
    max-width: 900px;
    margin: 0 auto;
    span{
      margin: 0 1em;
    }
  }
  .social{
    display: flex;
    align-items: center;
    color: blue;
    img{
      padding: .7em;
      max-width: 12%;
    }
  }
}
</style>
