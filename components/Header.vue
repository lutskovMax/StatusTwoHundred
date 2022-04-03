<template>
  <header class="header">
    <div class="container">
      <div class="header__body">
        <div class="header__logo">
          <img src="~@/assets/image/logo.png" alt="" />
        </div>
        <div class="header__menu">
          <ul>
            <nuxt-link to="/login">Питання</nuxt-link>
            <li>Позначки</li>
            <li>Учасники</li>
          </ul>
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