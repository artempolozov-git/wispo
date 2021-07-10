<template>
  <div class="header-catalog">
    <div class="catalog-icon"><img src="@/assets/icons/catalog.svg"></div>
    <div class="catalog-navigation">
      <div class="select-product">
        <div class="icon"><img src="@/assets/icons/smartphones.svg"></div>
        <select class="list" name="Устройство:">
          <option value="Смартфоны">Смартфоны</option> <!--Чтобы покрасить стрелочку в зеленый цвет, нашел способ заменить её через свойство background-->
        </select>
      </div>
      <div class="select-product">
        <div class="icon" style="width: 25px"><img src="@/assets/icons/pc.svg"></div>
        <select class="list" name="Устройство:">
          <option value="Планшеты и ПК">Планшеты и ПК</option>
        </select>
      </div>
      <div class="select-product">
        <div class="icon"><img src="@/assets/icons/smart.svg"></div>
        <select class="list" name="Устройство:">
          <option value="Умные устройства">Умные устройства</option>
        </select>
      </div>
      <div class="select-product">
        <div class="icon"><img src="@/assets/icons/gadgets.svg"></div>
        <select class="list" name="Устройство:">
          <option value="Гаджеты">Гаджеты</option>
        </select>
      </div>
      <div class="select-product">
        <div class="icon"><img src="@/assets/icons/audio.svg"></div>
        <select class="list" name="Устройство:">
          <option value="Аудиотехника">Аудиотехника</option>
        </select>
      </div>
      <div class="select-product">
        <div class="icon"><img src="@/assets/icons/other.svg"></div>
        <select class="list" name="Устройство:">
          <option value="Другое">Другое</option>
        </select>
      </div>
    </div>
    <button class="service-button" type="button"><img class="button-logo" src="@/assets/icons/white-logo.svg"></button>
  </div>
</template>

<script>
    export default {
        name: "HeaderCatalog"
    }
</script>

<style scoped>
.header-catalog {
  display: flex;
  align-items: center;
  box-sizing: border-box;
  max-width: 1520px;
  padding: 25px 0 25px 0;
  border-top: 1px solid #e6e6e6;
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
.select-product {
  display: flex;
  margin-left: 45px;
}
.icon {
  width: 20px;
  margin-right: 10px;
}
.list {
  font-family: Montserrat;
  font-weight: 500;
  font-size: 16px;
  border: none;
  outline: none;
  cursor: pointer;
}
.service-button {
  width: 170px;
  padding: 12px 18px 12px 18px;
  border-radius: 5px;
  box-sizing: border-box;
  margin-left: auto;
  border: none;
  outline: none;
  background-color: #000000;
  cursor: pointer;
}
</style>