<template>
  <footer>
    <div class="container">
      <div class="footer__body">
        <h3>© Форум "StatusTwoHundred" - всі права захищено</h3>
        <img src="~@/assets/image/logo.png" width="170" alt="" />
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  background: #f2f2f2;
  box-shadow: 0px -2px 18px rgb(0 0 0 / 25%);
  padding: 16px;
  max-height: 100vh;
}

h3 {
  color: #94b189;
}
.footer__body {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>