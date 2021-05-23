<template>
<header class="container">
  <div class="container-logo">
    <a href="/">
      <img src="../assets/img/dc-logo.png" alt="Logo">
    </a>
  </div>

  <div class="container-nav">
    <nav>
      <ul>
        <li v-for="(link, index) in menu" :key="index">
          <a :class="{'active': link.current}" :href="link.url">{{link.text}}</a>
        </li>
      </ul>
    </nav>
  </div>
</header> 
</template>

<script>
export default {
  name: 'HeaderComp',
    props:{
      menu:Array
    },
  data(){
    return{
      links: [],
    }
  }
}
</script>

<style lang="scss" scoped> // ^ abc
@import '../assets/style/vars.scss';

header{
  height: 120px;
  display: flex;
  align-items: center;
}

.container-logo{
  width: 35%;
}

.container-nav{
  width: auto;

  nav{
    width: 100%;
  }
}

ul{
  display: flex;
  width: 100%;
  justify-content: right;
  margin: 2rem 0;
  font-size: 0.85rem;

  a{
    padding: 1rem;
    color: rgb(79, 76, 72);
    text-transform: uppercase;
    &:hover,
    &.active{
      padding-bottom: 48px;
      border-bottom: 5px solid $blue-dc;
    }
  }
}
</style>