<template>
  <div id="app" class="container-fluid g-0">
    <Header />
    <ListCd />

  </div>
</template>

<script>
import Header from './components/Header.vue';
import ListCd from './components/ListCd.vue';

export default {
  name: 'App',
  components: {
    Header,
    ListCd
  }
}
</script>

<style lang="scss">
@import './styles/generals.scss';

.container-fluid {
  background: #1E2D3B;
  // height: 100%;
  height: 100vh;
  // position: relative;
}

</style>
