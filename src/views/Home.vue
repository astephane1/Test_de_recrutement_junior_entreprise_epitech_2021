<template>
  <div class="home" id="home">
    <img alt="Vue logo" src="../assets/career_center.png">
    <HelloWorld msg="Welcome to Career Center"/>
    <router-link to="/about">
    <button type="button" class="btn btn-outline-warning btn-lg btn-block">
        ENTER</button>
        </router-link>
        <router-view/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style scoped lang="scss">

#home button {
    display: inline-block;
    position: relative;
   left: 1%;
  top: 50px;
font-family: Avenir, Helvetica, Arial, sans-serif;
  font-weight: 700;
  //font-display: fallback;
    width: 250px;
    height: 100px;
}

#home img {
  height:50%;
  width:50%;
}
</style>
