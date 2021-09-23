<template>
  <div class="wrapper text-center">
    <div class="wrapper-cd">
      <img class="mb-3" :src="info.poster" alt="">
      <h2> {{info.title}} </h2>
      <h4> {{info.author}} </h4>
      <h6> {{info.year}} </h6>
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

 h2 {
      margin-bottom: 20px;
    }

 h4,
 h6 {
   color: grey;
   margin-bottom: 0px;
 }   

.wrapper {
  height: 450px;
  width: 100%;
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
