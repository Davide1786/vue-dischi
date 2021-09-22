<template>
  <div class="header">
    <img src="@/assets/img/Logo-Spoty.png" alt="">
    
  </div>
</template>

<script>
export default {
  name: 'Header',
  // props: {
  //   msg: String
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .header {
    width: 100%;
    height: 80px;
    background: #2E3A46;
      img {
        height: 100%;
        padding: 10px;
      }
  }
</style>
