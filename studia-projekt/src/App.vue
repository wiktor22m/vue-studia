<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld @click="handleChangeText" :text="content" />
  <WSB v-if="clicked"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import WSB from './components/WSB.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    WSB
  },
  data() {
    return {
      content: "WEB",
      clicked:false
    }
  },
  methods: {
    handleChangeText() {
      this.content = "strona",
      this.clicked = true
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
