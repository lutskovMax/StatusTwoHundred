<template>
  <div class="tags">
    <div class="tags__body">
      <h2>Нещодавні позначки</h2>
      <div class="tags__name">
        <nuxt-link to='/' v-for="tag in tags" :key="tag" class="tags__item tag">
          <span class="tag__body">{{ tag }} </span>
          <span class="tag__number"> x24 </span>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tags: [
        'python',
        'javascript',
        'html',
        'css',
        'c#',
        'reactjs',
        'java',
        'python-3.x',
        'pyqt5',
        'android',
        'svg',
        'php',
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.tags__body {
  padding-top: 74px;
}

h2 {
  margin-bottom: 32px;
}

.tags__name {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.tags__item {
  font-size: 16px;
  line-height: 1.2;
}

.tags {
    border-right: 1px solid #C4C4C4;
    padding-right: 46px;
    display: inline-block;
    padding-bottom: 74px;
}

.tag__number {
  font-size: 14px;
  line-height: 1.2;
  color: #727272;
}

.tag__body {
  color: #89b682;
  padding: 7px 13px;
  margin-bottom: 12px;
  background: #d3e6d0;
  border-radius: 5px;
  display: inline-block;
  transition: 0.2s;

  &:hover {
      background-color: #89b682;
      color: #fff;
  }
}
</style>