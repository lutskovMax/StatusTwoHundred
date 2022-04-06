<template>
  <div class="search">
    <div class="search__body">
      <h1>Досліджуйте питання на сайті</h1>
      <div class="input__body">
        <input class="search__input" type="text" placeholder="Пошук..." />
      </div>
      <button class="search__btn">Запитайте</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
h1 {
  font-size: 33px;
  line-height: 1.2;
  margin-bottom: 74px;
}

.search {
    padding-top: 150px;
    text-align: center;
}

.search__input {
  width: 555px;
  border: 1px solid #bcbcbc;
  border-radius: 3px;
  font-size: 13px;
  color: #727272;
  padding: 9px;
  margin-bottom: 74px;
}

.search__btn {
  background: #89b682;
  padding: 9px 29px;
  box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.25);
  border-radius: 5px;
  font-size: 16px;
  line-height: 1.2;
  color: #ffffff;
  transition: 0.2s;

  &:hover {
    background: #94b189;
  }
}
</style>
