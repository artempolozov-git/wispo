<template>
  <div class="categories-container">
    <div class="categories-panel">
      <div class="for-categories">
        <span>Для категорий</span>
        <img class="questions-icon" src="@/assets/icons/questions.svg">
      </div>
      <form action="" class="select-devices">
        <select class="list" name="Устройство:">
          <option value="Смартфоны">Смартфоны</option>
        </select>
      </form>
      <form action="" class="choose-parameters">
        <p class="parameters"><input name="select" id="characteristics" type="radio" value="Характеристики" checked> <!--Чтобы стилизовать кружок в зеленый цвет, нашел способ использовать псевдоклассы и абсолютное позиционирование, но не уверен в правильности решения, оставил как есть-->
          <label for="characteristics">Все характеристики</label>
        </p>
        <p class="parameters"><input name="select" id="differences" type="radio" value="Различия">
          <label for="differences"> Показать только различия</label>
        </p>
      </form>
    </div>
    <div class="selected-first-devices">
      <div class="close-icon"><img src="@/assets/icons/close-icon.svg"></div>
      <div class="compare-block">
        <div class="device-images-first"></div>
        <div class="device-info">
          <div class="category-title">Смартфоны</div>
          <div class="device-name">Apple iPhone 11 64 Gb (Gold)</div>
          <div class="price">49 999₽ <strike>60 999₽</strike></div>
          <div class="buy-controls">
            <a class="button-basket" href="#">В корзину</a>
            <div class="buy-one-click">
              <img src="@/assets/icons/phone-buy.svg">
              <span>Купить в 1 клик</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="selected-second-devices">
      <div class="close-icon"><img src="@/assets/icons/close-icon.svg"></div>
      <div class="compare-block">
        <div class="device-images-second"></div>
        <div class="device-info">
          <div class="category-title">Смартфоны</div>
          <div class="device-name">Xiaomi Redmi Note 8 Pro (blue)</div>
          <div class="price">16 700₽ <strike>19 999₽</strike></div>
          <div class="buy-controls">
            <a class="button-basket" href="#">В корзину</a>
            <div class="buy-one-click">
              <img src="@/assets/icons/phone-buy.svg">
              <span>Купить в 1 клик</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "DeviceCategory"
    }
</script>

<style scoped>
.categories-container {
  display: flex;
  align-items: center;
  padding-bottom: 25px;
  box-sizing: border-box;
  border-bottom: 2px solid #e6e6e6;
}
.categories-panel {
  display: block;
  margin-right: 90px;
}
.for-categories {
  display: flex;
  align-items: center;
  font-weight: 500;
  font-size: 16px;
}
.questions-icon {
  width: 24px;
  margin-left: 10px;
  cursor: pointer;
}
.list {
  width: 250px;
  padding: 20px 16px;
  margin-top: 20px;
  box-sizing: border-box;
  font-family: Montserrat;
  font-weight: 500;
  font-size: 16px;
  background: #FFFFFF;
  box-shadow: inset 3px 3px 3px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  color: #9A9A9A;
  border: 1px solid #F0F2F4;
  outline: none;
  cursor: pointer;
}
.choose-parameters {
  margin-top: 30px;
  font-weight: 400;
  font-size: 16px;
}
.parameters >  input, label{
  cursor: pointer;
  margin-right: 10px;
}
.close-icon {
  display: flex;
  justify-content: flex-end;
  cursor: pointer;
}
.selected-second-devices {
  margin-left: 170px;
}
.select-devices {
  display: flex;
  align-items: center;
}
.compare-block {
  display: flex;
}
.device-images-first {
  width: 120px;
  height: 150px;
  margin-right: 30px;
  background: url(../assets/images/iphone.png);
  background-size: cover;
  background-position: center;
}
.device-images-second {
  width: 120px;
  height: 150px;
  margin-right: 30px;
  background: url(../assets/images/xiaomi.png);
  background-size: cover;
  background-position: center;
}
.device-info {
  display: block;
}
.category-title {
  font-weight: 400;
  color: #9A9A9A;
  margin-bottom: 15px;
}
.device-name {
  font-weight: 500;
  font-size: 16px;
  margin-bottom: 20px;
}
.price {
  font-weight: 600;
  font-size: 20px;
}
.price > strike {
  font-weight: 500;
  font-size: 14px;
  color: #9A9A9A;
}
.buy-controls {
  display: flex;
  align-items: center;
  margin-top: 10px;
}
.button-basket {
  padding: 12px 18px 12px 18px;
  box-sizing: border-box;
  border-radius: 10px;
  text-decoration: none;
  background-color: #000000;
  cursor: pointer;
  text-align: center;
  font-family: Montserrat;
  font-weight: 600;
  font-size: 14px;
  color: #FFFFFF;
}
.buy-one-click {
  display: flex;
  align-items: center;
  margin-left: 20px;
  cursor: pointer;
}
.buy-one-click > span {
  font-weight: 600;
  margin-left: 10px;
}
@media only screen and (max-width : 1536px) {
  .compare-block {
    display: block;
  }
  .selected-second-devices {
    margin-left: 100px;
  }
  .device-info {
    margin-top: 20px;
  }
}
@media only screen and (max-width : 980px) {
  .categories-panel {
    margin-right: 20px;
  }
  .buy-controls {
    display: block;
    margin-top: 30px;
  }
  .buy-one-click {
    margin: 0;
    margin-top: 30px;
  }
}
@media only screen and (max-width : 768px) {
  .for-categories {
    font-size: 12px;
  }
  .list {
    width: 180px;
    padding: 15px 16px;
    font-size: 10px;
  }
  .choose-parameters {
    font-size: 12px;
  }
  .selected-second-devices {
    margin-left: 60px;
  }
}
@media only screen and (max-width : 533px) {
  .categories-container {
    display: block;
  }
  .device-images-first {
    margin: auto;
  }
  .category-title {
    text-align: center;
  }
  .device-name {
    text-align: center;
    font-size: 14px;
  }
  .price {
    font-size: 16px;
    text-align: center;
  }
  .buy-one-click {
    display: none;
  }
  .buy-controls {
    display: flex;
    justify-content: center;
    margin: 20px 0 20px 0;
  }
  .selected-second-devices {
    margin: 0;
  }
  .device-images-second {
    margin: auto;
  }
}
</style>