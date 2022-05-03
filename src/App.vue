<template>
  <div id="app">
 
    <HeaderSite/>
    <MainSite/>
    <FooterSite/>
    
  </div>
</template>

<script>
import 'bootstrap';
import 'bootstrap/dist/css/bootstrap.min.css';
import HeaderSite from '@/components/HeaderComponent';
import MainSite from '@/components/MainComponent';
import FooterSite from '@/components/FooterComponent';


export default {
  name: 'App',
  components: {
    HeaderSite,
    MainSite,
    FooterSite
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

</style>
