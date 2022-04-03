<template>
  <div class="wrapper">
    <Header />
    <h1>Nice</h1>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',

  mounted() {
    this.$axios
      .get('https://webforum.azurewebsites.net/api/Values')
      .then((r) => {
        console.log(r.data)
      })
  },
}
</script>
<style lang="scss" scoped>
h1 {
  color: aqua;
}
</style>
