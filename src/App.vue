<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <ui-button>
    Контент из app
  </ui-button>


  <service-item>
    
  </service-item>



</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import UiButton from './components/UiButton.vue';
import ServiceItem from './components/ServiceItem.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    UiButton,
    ServiceItem,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
