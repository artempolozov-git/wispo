<template>
  <div class="header-navigation">
    <div class="select-city">
      <div class="icon"><img src="@/assets/icons/location.svg"></div>
      <select class="list" name="Город:">
        <option value="Челябинск">Челябинск</option> <!--Чтобы покрасить стрелочку в зеленый цвет, нашел способ заменить её через свойство background-->
      </select>
    </div>
    <div class="nav-address">
      <nav>Адреса</nav>
    </div>
    <div class="rating"><img src="@/assets/icons/rating.svg"></div> <!--Можно сделать облачко с помощью css свойст, но пришлось бы возиться с абсолютным позиционированием, псевдоклассами и вычеслениями, но это увеличивает код и может привести к тому, что блок съедет -->
    <div class="nav-links">
      <nav class="navigation">Как купить</nav>
      <nav class="navigation">О нас</nav>
      <nav class="navigation">Акции</nav>
      <nav class="navigation">Контакты</nav>
    </div>
    <div class="time-works">
      <span>c 7:00 до 20:00</span>
    </div>
    <div class="phone-contact">
      <img src="@/assets/icons/phone.svg">
      <a href="tel:+73517014087" class="phone">+7 351 701 40 87</a>
    </div>
    <div class="messengers-contacts">
      <div class="wa-msg"><img src="@/assets/icons/whatsapp.svg"></div>
      <div class="viber-msg"><img src="@/assets/icons/viber.svg"></div>
      <div class="tg-msg"><img src="@/assets/icons/telegram.svg"></div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "HeaderNavigation"
    }
</script>

<style scoped>
.header-navigation {
  display: flex;
  align-items: center;
  justify-content: center;
  box-sizing: border-box;
  max-width: 1520px;
  padding: 22px 0 22px 0;
  margin: auto;
  height: 76px;
}
.select-city {
  display: flex;
  align-items: center;
}
.icon {
  width: 15px;
  margin-right: 10px;
}
.list {
  font-family: Montserrat;
  font-weight: 600;
  border: none;
  outline: none;
  cursor: pointer;
}
.nav-address {
  font-weight: 400;
  margin: 0 30px 0 30px;
  border-bottom: 2px solid #e6e6e6;
  cursor: pointer;
}
.rating {
  width: 220px;
}
.nav-links {
  display: flex;
  align-items: center;
  margin-left: 30px;
}
.navigation {
  font-weight: 400;
  margin-right: 30px;
  border-bottom: 2px solid #e6e6e6;
  cursor: pointer;
}
.time-works {
  margin-left: 120px;
  font-weight: 500;
  color: #9A9A9A;
}
.phone-contact {
  display: flex;
  align-items: center;
  margin: 0 20px 0 25px;
}
.phone {
  font-size: 20px;
  font-weight: 600;
  margin-left: 15px;
  text-decoration: none;
  color: #000000;
}
.messengers-contacts {
  display: flex;
  align-items: center;
}
.wa-msg {
  display: flex;
  align-items: center;
  width: 25px;
  height: 15px;
  padding: 0 20px 0 20px;
  border-left: 2px solid #e6e6e6;
  border-right: 2px solid #e6e6e6;
  cursor: pointer;
}
.viber-msg {
  display: flex;
  align-items: center;
  padding: 0 20px 0 20px;
  cursor: pointer;
}
.tg-msg {
  display: flex;
  align-items: center;
  height: 15px;
  padding: 0 20px 0 20px;
  border-left: 2px solid #e6e6e6;
  border-right: 2px solid #e6e6e6;
  cursor: pointer;
}
</style>