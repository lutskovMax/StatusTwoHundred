<template>
  <header class="header">
    <div class="container">
      <div class="header__body">
        <div class="header__logo">
          <img src="~@/assets/image/logo.png" alt="" />
        </div>
        <div class="header__menu">
          <ul>
            <li><nuxt-link to="/login">Питання</nuxt-link></li>
            <li><nuxt-link to="/">Позначки</nuxt-link></li>
            <li><nuxt-link to="/">Учасники</nuxt-link></li>
          </ul>
        </div>
        <div class="header__login">
          <nuxt-link class="btn_in header__btn" to="/login">Вхід</nuxt-link>
          <nuxt-link class="btn_out header__btn" to="/login"
            >Реєстрація</nuxt-link
          >
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  methods: {
    localePathAbout() {
      return this.localePath('login')
    },
  },
}
</script>

<style scoped lang="scss">
.header {
  background: #f2f2f2;
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.25);
  padding: 16px;
  &__body {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__menu {
    ul {
      display: flex;
      color: #727272;
      font-size: 18px;
      line-height: 1.2;
      li {
        margin-right: 26px;

        a {
          color: #727272;
        }
      }
    }
  }

  &__login {
    .header__btn {
      font-size: 16px;
      border: 1px solid #89b682;
      border-radius: 5px;
    }

    .btn_in {
      background: #dadada;
      padding: 9px 21px;
      color: #89b682;
    }

    .btn_out {
      padding: 9px 21px;
      color: #fff;
      background: #89b682;
      box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.25);
      border-radius: 5px;
      margin-left: 11px;
    }
  }
}
</style>