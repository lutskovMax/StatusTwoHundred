<template>
  <div class="questions">
    <div class="questions__body">
      <h2>Останні питання</h2>
      <div class="questions__items">
        <nuxt-link to='/' v-for="quest in questions" :key="quest" class="questions__name">
          {{ quest }}
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      questions: [
        'Як видалити всі залежні packsge.json?',
        'Не працює код на python',
        'Як видалити всі залежні packsge.json?',
        'Не працює код на python',
        'Як видалити всі залежні packsge.json?',
        'Не працює код на python',
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.questions {
    border-left: 1px solid #C4C4C4;
    padding-left: 46px;
}
.questions__body {
  padding-top: 74px;
}

h2 {
  margin-bottom: 32px;
}

.questions__name {
  font-size: 16px;
  line-height: 1.2;
  color: #94b189;
  max-width: 190px;
  margin-left: 22px;
  position: relative;
  margin-bottom: 29px;
  display: block;
  transition: 0.2s;

  &:hover {
      color: #89b682;
      font-weight: 700;
  }

  &::before {
      position: absolute;
      content: '';
      width: 10px;
      height: 10px;
      left: -22px;
      top: 3px;
      background: #89B682;
      border-radius: 50%;
  }
}
</style>