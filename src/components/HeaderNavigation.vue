<template>
  <div class="header-navigation">
    <div class="dropdown">
      <div class="dropdown-button">
        <div class="icon"><img src="@/assets/icons/location.svg"></div>
        <span class="dropdown-title">Челябинск</span>
        <div class="dropdown-icon"><img src="@/assets/icons/dropdown-arrow.svg"></div>
      </div>
      <div class="dropdown-content">
        <a href="#">Москва</a>
        <a href="#">Воронеж</a>
      </div>
    </div>
    <div class="nav-address">
      <nav>Адреса</nav>
    </div>
    <div class="rating"><img src="@/assets/icons/rating.svg"></div>
    <div class="dropdown-information">
      <div class="dropdown-button" href="#">
        <span class="dropdown-title">Информация</span>
        <div class="dropdown-icon"><img src="@/assets/icons/dropdown-arrow.svg"></div>
      </div>
      <div class="dropdown-content">
        <a href="#">Как купить</a>
        <a href="#">О нас</a>
        <a href="#">Акции</a>
        <a href="#">Контакты</a>
      </div>
    </div>
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
  box-sizing: border-box;
  max-width: 1520px;
  padding: 22px 0 22px 0;
  margin: auto;
  height: 76px;
}
.icon {
  width: 15px;
  margin-right: 10px;
}
.dropdown-title {
  font-family: Montserrat;
  font-weight: 600;
  font-size: 14px;
  margin: 0 10px;
}
.nav-address {
  font-weight: 400;
  margin: 0 30px 0 30px;
  border-bottom: 2px solid #e6e6e6;
  cursor: pointer;
}
.rating {
  width: 220px;
  cursor: pointer;
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
  margin-left: 100px;
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
.dropdown-button {
  display: flex;
  align-items: center;
  background-color: #FFFFFF;
  text-decoration: none;
  color: #000000;
}
.dropdown {
  position: relative;
  display: inline-block;
}
.dropdown-information {
  position: relative;
  display: none;
}
.dropdown-content {
  display: none;
  position: absolute;
  border-radius: 5px;
  background-color: #FFFFFF;
  width: 100%;
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
  padding: 12px 16px;
}
.dropdown:hover .dropdown-content {
  display: block;
}
.dropdown:hover .dropdown-button {
  cursor: pointer;
}
@media only screen and (max-width : 1536px) {
  .header-navigation {
    max-width: 1080px;
  }
  .nav-links {
    display: none;
  }
  .nav-address {
    display: none;
  }
  .wa-msg, .tg-msg, .viber-msg {
    padding: 0 10px 0 10px;
  }
  .dropdown-information {
    position: relative;
    display: inline-block;
  }
  .dropdown-information:hover .dropdown-content {
    display: block;
  }
  .dropdown-information:hover .dropdown-button {
    cursor: pointer;
  }
  .rating {
    margin: 0 20px 0 20px;
  }
  .time-works {
    margin-left: 70px;
  }
}
@media only screen and (max-width : 980px) {
  .header-navigation {
    max-width: 850px;
  }
  .time-works {
    display: none;
  }
  .messengers-contacts {
    display: none;
  }
  .phone-contact {
    margin: 0;
    margin-left: auto;
  }
}
@media only screen and (max-width : 768px) {
  .header-navigation {
    max-width: 650px;
  }
  .rating {
    display: none;
  }
  .dropdown-information {
    margin-left: 20px;
  }
}
@media only screen and (max-width : 533px) {
  .header-navigation {
    max-width: 320px;
  }
  .phone-contact {
    display: none;
  }
  .header-navigation {
    justify-content: center;
  }
}
</style>