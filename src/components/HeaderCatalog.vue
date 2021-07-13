<template>
  <div class="header-catalog">
    <div class="catalog-container">
      <div class="catalog-icon"><img src="@/assets/icons/catalog.svg"></div>
      <div class="dropdown-catalog">
        <div class="dropdown-button">
          <span class="dropdown-title">Каталог</span>
          <div class="dropdown-icon"><img src="@/assets/icons/dropdown-arrow.svg"></div>
        </div>
        <div class="dropdown-content">
          <a href="#">Смартфоны</a>
          <a href="#">Планшеты и ПК</a>
          <a href="#">Умные устройства</a>
          <a href="#">Гаджеты</a>
          <a href="#">Аудиотехника</a>
          <a href="#">Другое</a>
        </div>
      </div>
      <div class="search">
        <input class="search-input" type="text" placeholder="Искать технику">
        <a class="search-button" href="#"><img class="search-icon" src="@/assets/icons/search-icon.svg"><span>Найти</span></a> <!--Можно добавить кнопку в инпут с помощью абсолютного позиционирования, но я сделал это с помощью стилей-->
      </div>
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
        <div class="dropdown" id="audio">
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
.dropdown-catalog {
  position: relative;
  display: none;
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
.search {
  display: none;
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
@media only screen and (max-width : 1536px) {
  .catalog-container {
    max-width: 1080px;
  }
  #audio {
    display: none;
  }
  .catalog-icon {
    padding-right: 20px;
  }
  .dropdown {
    margin-left: 20px;
  }
  .icon {
    width: 15px;
  }
}
@media only screen and (max-width : 980px) {
  .catalog-container {
    max-width: 850px;
  }
  .catalog-navigation {
    display: none;
  }
  .catalog-icon {
    border: none;
  }
  .dropdown-button {
    font-weight: 600;
    text-decoration: none;
  }
  .dropdown-icon {
    margin-left: 10px;
  }
  .dropdown-catalog {
    position: relative;
    display: inline-block;
  }
  .dropdown-catalog:hover .dropdown-content {
    display: block;
  }
  .dropdown-catalog:hover .dropdown-button {
    cursor: pointer;
  }
  .dropdown-content {
    width: 180px;
  }
  .search {
    display: flex;
  }
  .search-input {
    padding: 15px 10px 15px 20px;
    width: 345px;
  }
  .search-button {
    padding: 15px 40px 15px 0;
    margin-right: 30px;
  }
}
@media only screen and (max-width : 768px) {
  .catalog-container {
    max-width: 650px;
  }
  .search-input {
    width: 215px;
  }
  .search-button {
    padding: 15px 20px 15px 0;
  }
  .search-button > span {
    display: none;
  }
}
@media only screen and (max-width : 533px) {
  .catalog-container {
    max-width: 320px;
    justify-content: center;
  }
  .service-button {
    display: none;
  }
  .search-input {
    width: 120px;
    margin-left: 10px;
  }
  .search-button {
    margin: 0;
  }
  .search-icon {
    margin: 0;
  }
  .catalog-icon {
    padding-right: 10px;
  }
}
</style>