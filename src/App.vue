<template>

  <service-item></service-item>
    <my-alert
      title="Did you know?"
      intent="danger"
      :show="showInfo"
      :on-dismiss="() => (showInfo = false)"
    >
    <p class="mb-2">
      You subscribing to my youtube channel keeps me motivated to create more
      components?
    </p>
    <p>
      Click
      <a
        class="font-semibold text-blue-700 underline"
        href="https://youtube.com/ConstantinDruc"
      >
        here
      </a>
      to subscribe!
    </p>
  </my-alert>
</template>

<script>
import ServiceItem from './components/ServiceItem.vue';
import MyAlert from './components/MyAlert.vue';

export default {
  name: 'App',
  components: {
    ServiceItem,
    MyAlert,
  },
  data(){
    return {
      ticker: 'default2',
    }
  },
  methods: {
    add(){
      alert(this.ticker);
    }
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
