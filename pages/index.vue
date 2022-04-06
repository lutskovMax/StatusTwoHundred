<template>
  <div class="wrapper">
    <Header />

    <div class="main__page">
      <Main />
    </div>
    <Footer />
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
.wrapper {
      display: flex;
    flex-direction: column;
    justify-content: space-between;
}
</style>
