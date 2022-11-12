<template>
  <div class="hello">
    <h1 >{{ contentHC }}</h1>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    text: String
  },
  data() {
    return { contentHC: this.text }
  },
  watch: {
    text(nVal) {
      return this.contentHC = nVal
    }
  }

}
</script>

