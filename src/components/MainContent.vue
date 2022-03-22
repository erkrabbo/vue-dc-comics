<template>
  <div>
      <span>-->Content goes here</span>
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: 'MainContent'
    }
  }
}
</script>

<style scoped lang="scss">
div{
    background-color: black;
    color: white;
    height: 5rem;
    display: flex;
    align-items: center;
    span{
        display: inline-block;
        width: 900px;
        margin: 0 auto;
    }
}
</style>
