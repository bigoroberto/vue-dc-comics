<template>
  <div id="app">
    <HeaderComp :menu="links"/>
    <MainComp/>
    <FooterComp/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import FooterComp from './components/FooterComp.vue'
export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp
  },
  data(){
    return{
      links:[
                {
          text: 'Characters',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Comics',
          url: 'javascript:void(0)',
          current: true
        },
        {
          text: 'Movies',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Tv',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Games',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Collectibles',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Videos',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Fans',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'News',
          url: 'javascript:void(0)',
          current: false
        },
        {
          text: 'Shop',
          url: 'javascript:void(0)',
          current: false
        },
      ]
    }
  }
}
</script>


<style lang="scss">
@import './assets/style/general.scss';
@import './assets/style/utilities.scss'
</style>