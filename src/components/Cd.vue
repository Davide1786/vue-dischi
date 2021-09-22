<template>
  <div class="wrapper text-center">
    <div class="wrapper-cd">
      <img class="mb-3" :src="info.poster" :alt="info.title">
      <h4> {{info.author}} </h4>
      <div> {{info.year}} </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Cd',
  props: ['info']
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.wrapper {
  display: flex;
  height: 350px;
  margin-bottom: 20px;
  flex-direction: column;
  background: #2E3A46;

    .wrapper-cd {
      height: 50%;
      width: 100%;
      padding: 20px;
      
        img {
          width: 100%;
        }
    }
}
</style>
