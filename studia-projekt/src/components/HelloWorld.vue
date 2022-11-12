<template>
  <div class="hello">
    <h1 @click="handleChangeText">{{ name }}</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'WEB'
    }
  },
  methods: {
    handleChangeText() {
      this.name = "strona"
    }
  }
}
</script>

