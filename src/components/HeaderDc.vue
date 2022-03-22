<template>
  <nav>
      <img src="../assets/img/dc-logo.png" alt="DC logo">
      <ul>
          <li v-for="(link, index) in navLinks" :key="index" @click="changeActive(index)" :class="{active: activeIndex == index}"><a :href="link.href">{{ link.text }}</a></li>
      </ul>
  </nav>
</template>

<script>
export default {
  data () {
    return {
      activeIndex: 0,
      navLinks: [
        {
          href: '#',
          text: 'CHARACTERS'
        },
        {
          href: '#',
          text: 'COMICS'
        },
        {
          href: '#',
          text: 'MOVIES'
        },
        {
          href: '#',
          text: 'TV'
        },
        {
          href: '#',
          text: 'GAMES'
        },
        {
          href: '#',
          text: 'COLLECTIBLES'
        },
        {
          href: '#',
          text: 'VIDEOS'
        },
        {
          href: '#',
          text: 'FANS'
        },
        {
          href: '#',
          text: 'NEWS'
        },
        {
          href: '#',
          text: 'SHOP'
        }
      ]
    }
  },
  methods: {
    changeActive (index) {
      this.activeIndex = index
    }
  }
}
</script>

<style scoped lang="scss">
    nav{
        display: flex;
        // align-items: center;
        ul{
            list-style: none;
            display: flex;
            li{
                display: flex;
                align-items: center;
                border-bottom: .5em solid transparent;
                    &.active{
                        border-bottom-color: blue;
                        a{
                            color: blue;
                        }
                    }
                a{
                    display: block;
                    text-decoration: none;
                    color: #4d4654;
                    padding: 1rem;
                }
            }
        }
        img{
            margin-right: auto;
        }
    }
</style>
