<template>
  <div class="header-panel">
    <div class="logotype"><img src="@/assets/icons/logotype.svg"></div>
    <div class="search">
      <input class="search-input" type="text" placeholder="Искать технику">
      <a class="search-button" href="#"><img class="search-icon" src="@/assets/icons/search-icon.svg"><span>Найти</span></a> <!--Можно добавить кнопку в инпут с помощью абсолютного позиционирования, но я сделал это с помощью стилей-->
    </div>
    <div class="control-panel">
      <a class="panel-button" href="#" id="comparison">
        <div class="control-icon"><img src="@/assets/icons/comparison.svg"></div>
        <span>Сравнение</span>
      </a>
      <a class="panel-button" href="#" id="favorites">
        <div class="control-icon"><img src="@/assets/icons/favorites.svg"></div>
        <span>Избранное</span>
      </a>
      <a class="panel-button" href="#">
        <div class="control-icon"><img src="@/assets/icons/cabinet.svg"></div>
        <span>Мой кабинет</span>
      </a>
      <a class="panel-button" href="#">
        <div class="control-icon"><img src="@/assets/icons/basket.svg"></div>
        <span>Корзина</span>
      </a>
    </div>
  </div>
</template>

<script>
    export default {
        name: "HeaderPanel"
    }
</script>

<style scoped>
.header-panel {
  display: flex;
  align-items: center;
  box-sizing: border-box;
  max-width: 1520px;
  padding: 22px 0 22px 0;
  margin: 0 auto 15px;
  height: 76px;
}
.logotype {
  width: 350px;
  cursor: pointer;
}
.search {
  display: flex;
  align-items: center;
}
.search-input {
  font-family: Montserrat;
  font-weight: 500;
  font-size: 14px;
  width: 420px;
  margin-left: 30px;
  padding: 25px 10px 25px 40px;
  border-radius: 5px 0 0 5px;
  border: none;
  outline: none;
  background-color: #F6F6F6;
}
.search-button {
  display: flex;
  align-items: center;
  font-family: Montserrat;
  font-weight: 600;
  font-size: 14px;
  padding: 25px 40px 25px 0;
  border-radius: 0 5px 5px 0;
  text-decoration: none;
  background-color: #F6F6F6;
  color: #9A9A9A;
  cursor: pointer;
}
.search-icon {
  width: 15px;
  margin-right: 18px;
}
.control-panel {
  display: flex;
  align-items: flex-end;
}
.panel-button {
  margin-left: 45px;
  text-decoration: none;
  color: #000000;
  cursor: pointer;
}
.control-icon {
  width: 20px;
  margin: auto;
}
@media only screen and (max-width : 1536px) {
  .header-panel {
    max-width: 1080px;
  }
  .search-button > span {
    display: none;
  }
  .logotype {
    width: 300px;
  }
  .search-input {
    width: 150px;
    padding: 25px 10px 25px 20px;
  }
  .search-button {
    padding: 25px 20px 25px 0;
  }
  .search-icon {
    margin: 0;
  }
  .panel-button {
    margin-left: 30px;
  }
}
@media only screen and (max-width : 980px) {
  .header-panel {
    max-width: 850px;
  }
  .search {
    display: none;
  }
  .control-panel {
    margin-left: auto;
  }
}
@media only screen and (max-width : 768px) {
  .header-panel {
    max-width: 650px;
  }
  #comparison, #favorites {
    display: none;
  }
}
@media only screen and (max-width : 533px) {
  .header-panel {
    max-width: 320px;
    justify-content: center;
  }
  .panel-button > span{
    display: none;
  }
  .logotype {
    width: 180px;
  }
  .control-panel {
    margin: 0;
  }
}
</style>