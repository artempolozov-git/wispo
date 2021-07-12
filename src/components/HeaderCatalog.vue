<template>
  <div class="header-catalog">
    <div class="catalog-container">
      <div class="catalog-icon"><img src="@/assets/icons/catalog.svg"></div>
      <div class="catalog-navigation">
        <div class="dropdown">
          <div class="dropdown-button">
            <div class="icon"><img src="@/assets/icons/smartphones.svg"></div>
            <span class="list-title">Смартфоны</span>
            <div class="dropdown-icon"><img src="@/assets/icons/dropdown-arrow.svg"></div>
          </div>
          <div class="dropdown-content">
            <a href="#">iPhone</a>
            <a href="#">Xiaomi</a>
            <a href="#">Samsung</a>
          </div>
        </div>
        <div class="dropdown">
          <div class="dropdown-button">
            <div class="icon"><img src="@/assets/icons/pc.svg"></div>
            <span class="list-title">Планшеты и ПК</span>
            <div class="dropdown-icon"><img src="@/assets/icons/dropdown-arrow.svg"></div>
          </div>
          <div class="dropdown-content">
            <a href="#">Планшеты</a>
            <a href="#">Ноутбуки</a>
            <a href="#">ПК</a>
          </div>
        </div>
        <div class="dropdown">
          <div class="dropdown-button">
            <div class="icon"><img src="@/assets/icons/smart.svg"></div>
            <span class="list-title">Умные устройства</span>
            <div class="dropdown-icon"><img src="@/assets/icons/dropdown-arrow.svg"></div>
          </div>
          <div class="dropdown-content">
            <a href="#">Часы Apple</a>
            <a href="#">Станции Яндекс</a>
            <a href="#">Часы Samsung</a>
          </div>
        </div>
        <div class="dropdown">
          <div class="dropdown-button">
            <div class="icon"><img src="@/assets/icons/gadgets.svg"></div>
            <span class="list-title">Гаджеты</span>
            <div class="dropdown-icon"><img src="@/assets/icons/dropdown-arrow.svg"></div>
          </div>
          <div class="dropdown-content">
            <a href="#">Консоли</a>
            <a href="#">Камеры</a>
            <a href="#">Мышки</a>
          </div>
        </div>
        <div class="dropdown">
          <div class="dropdown-button">
            <div class="icon"><img src="@/assets/icons/audio.svg"></div>
            <span class="list-title">Аудиотехника</span>
            <div class="dropdown-icon"><img src="@/assets/icons/dropdown-arrow.svg"></div>
          </div>
          <div class="dropdown-content">
            <a href="#">Наушники</a>
            <a href="#">Колонки</a>
          </div>
        </div>
        <div class="dropdown">
          <div class="dropdown-button">
            <div class="icon"><img src="@/assets/icons/other.svg"></div>
            <span class="list-title">Другое</span>
            <div class="dropdown-icon"><img src="@/assets/icons/dropdown-arrow.svg"></div>
          </div>
          <div class="dropdown-content">
            <a href="#">Сумки</a>
            <a href="#">Рюкзаки</a>
          </div>
        </div>
      </div>
      <a class="service-button" href="#"><img class="button-logo" src="@/assets/icons/white-logo.svg"></a>
    </div>
  </div>
</template>

<script>
    export default {
        name: "HeaderCatalog"
    }
</script>

<style scoped>
.header-catalog {
  border-top: 1px solid #e6e6e6;
}
.catalog-container {
  display: flex;
  align-items: center;
  box-sizing: border-box;
  padding: 25px 0 25px 0;
  max-width: 1520px;
  margin: auto;
  height: 76px;
}
.catalog-icon {
  display: flex;
  align-items: center;
  padding-right: 45px;
  border-right: 2px solid #e6e6e6;
  width: 25px;
}
.catalog-icon > img {
  cursor: pointer;
}
.catalog-navigation {
  display: flex;
  align-items: center;
}
.icon {
  width: 20px;
}
.list-title {
  font-family: Montserrat;
  font-weight: 500;
  font-size: 16px;
  margin: 0 10px;
}
.service-button {
  width: 170px;
  padding: 12px 18px 12px 18px;
  border-radius: 5px;
  box-sizing: border-box;
  margin-left: auto;
  text-decoration: none;
  background-color: #000000;
  cursor: pointer;
}
.dropdown-button {
  display: flex;
  align-items: center;
  background-color: #FFFFFF;
  color: #000000;
}
.dropdown {
  position: relative;
  display: inline-block;
  margin-left: 45px;
}
.dropdown-content {
  display: none;
  position: absolute;
  border-radius: 5px;
  background-color: #FFFFFF;
  width: 100%;
  padding: 10px;
  box-shadow: 0px 5px 18px 2px rgba(230, 230, 230, 0.6);
  z-index: 1;
}
.dropdown-content a {
  font-family: Montserrat;
  font-weight: 500;
  font-size: 14px;
  color: black;
  box-sizing: border-box;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}
.dropdown-content a:hover {
  background-color: #f3f3f3;
}
.dropdown:hover .dropdown-content {
  display: block;
}
.dropdown:hover .dropdown-button {
  cursor: pointer;
}
</style>