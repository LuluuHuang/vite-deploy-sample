<template>
  <div class="about">
    <h1>This is an about page</h1>
    {{ data }}
  </div>
</template>

<script>
export default {
  data() {
    return {
      data: {}
    }
  },
  mounted() {
    console.log(import.meta.env.VITE_TEXT)
    const url = import.meta.env.VITE_PATH
    this.$http.get(url).then((response) => {
      console.log(response.data)
      this.data = response.data.results[0]
    })
  }
}
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
