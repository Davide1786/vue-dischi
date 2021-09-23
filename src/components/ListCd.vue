<template>
  <div class="container">
    <div class="row wrapper">
      <!-- TODO stampo lista personaggi -->
      <div v-for="(lista, index) in listaCd" :key="index" class="col-lg-2 testo">
         <Cd :info="lista"/>
      </div>
    </div>
    
  </div>
</template>

<script>
import axios from 'axios';
import Cd from '../components/Cd.vue';

export default {
  name: 'ListCd',
  components: {
    Cd
  },
  data() {
    return {
      APIUrl: 'https://flynn.boolean.careers/exercises/api/array/music',
      listaCd: []
    }
  },
  created() {
    this.getlistCd();
  },
  methods: {
    getlistCd() {
      axios
          .get(this.APIUrl)
          .then( res => {
            // console.log(res.data.response)
            this.listaCd = res.data.response;
          })
    }
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.container {
  display: flex;
  align-items: center;
  justify-content: center;
  justify-items: center;
  padding: 50px;
  
}

  .wrapper {
    flex-wrap: wrap;
    margin: 10px 5px;
    justify-items: center;
    
  }

    .testo {
      width: calc(100% / 5);
      color: white;
      justify-content: space-around;
    }
   

</style>
