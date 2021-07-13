<template>
  <div class="footer">
    <footer-feedback-section></footer-feedback-section>
    <div class="footer-main-container">
      <div class="company-info-block">
        <div class="footer-logo"><img src="@/assets/icons/footer-logo.svg"></div>
        <div class="info-about-company">
          <h2 class="copyrigh">2012-2020 © Белая Техника</h2>
          <h2 class="description-company">Интернет-магазин Белая Техника — российская розничная торговая сеть по продаже современной электроники.</h2>
        </div>
        <div class="yandex-rating"><img src="@/assets/icons/footer-rating.svg"></div>
        <div class="payment-systems">
          <div class="payment-info">Принимаем к оплате</div>
          <img src="@/assets/icons/payments.svg">
        </div>
      </div>
      <div class="contacts-navigations-container">
        <div class="company-contacts-block">
          <div class="number-phone">
            <div class="number">+7 351 701 40 87</div>
            <div class="time-works">Ежедневно 10:00-21:00</div>
          </div>
          <div class="callback-button">
            <a class="order-button" href="#">
              <img src="@/assets/icons/white-phone.svg">
              <span>Заказать звонок</span>
            </a>
          </div>
          <div class="feedback-messengers">
            <div class="viber-icon"><img src="@/assets/icons/footer-viber.svg"></div>
            <div class="wa-icon"><img src="@/assets/icons/footer-wa.svg"></div>
            <div class="tg-icon"><img src="@/assets/icons/footer-tg.svg"></div>
          </div>
        </div>
        <div class="navigations-main-block">
          <div class="navigation-menu">
            <div class="navigation-title">Каталог</div>
            <div class="navigation-link"><a href="#">Смартфоны</a></div>
            <div class="navigation-link"><a href="#">Планшеты и компьюетры</a></div>
            <div class="navigation-link"><a href="#">Умные часы и браслеты</a></div>
            <div class="navigation-link"><a href="#">Гаджеты</a></div>
            <div class="navigation-link"><a href="#">Аудиотехника</a></div>
            <div class="navigation-link"><a href="#">Другое</a></div>
            <div class="navigation-link"><a href="#">Топ гаджеты</a></div>
          </div>
          <div class="navigation-menu">
            <div class="navigation-title">Информация</div>
            <div class="navigation-link"><a href="#">О нас</a></div>
            <div class="navigation-link"><a href="#">Как купить</a></div>
            <div class="navigation-link"><a href="#">Акции</a></div>
            <div class="navigation-link"><a href="#">Контакты</a></div>
          </div>
          <div class="navigation-menu">
            <div class="navigation-title">Мы на связи</div>
            <div class="feedback-link">
              <img src="@/assets/icons/dzen.svg">
              <a href="#">Яндекс.Дзен</a>
            </div>
            <div class="feedback-link">
              <img src="@/assets/icons/service-icon.svg">
              <a href="#">Белый Сервис</a>
            </div>
            <div class="messengers-links">
              <a href="#" style="margin-right: 10px"><img src="@/assets/icons/insta-icon.svg"></a>
              <a href="#"><img src="@/assets/icons/vk-icon.svg"></a>
            </div>
          </div>
          <div class="navigation-menu" style="margin: 0">
            <div class="navigation-title">Адреса</div>
            <div class="location-link">
              <img src="@/assets/icons/location.svg">
              <span>Энгельса, д. 75</span>
            </div>
            <div class="location-link">
              <img src="@/assets/icons/location.svg">
              <span>Энгельса, д. 30</span>
            </div>
            <div class="location-link" style="border: none">
              <img src="@/assets/icons/location.svg">
              <span>Ул. Набережная, д. 80</span>
            </div>
            <div>
              <a class="location-button" href="#">На карте</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    import FooterFeedbackSection from "@/components/FooterFeedbackSection";
    export default {
        name: "Footer",
        components: {FooterFeedbackSection}
    }
</script>

<style scoped>
.footer {
  height: auto;
  background-color: #ffffff;
}
.footer-main-container {
  display: flex;
  box-sizing: border-box;
  padding: 60px 0 200px 0;
  max-width: 1520px;
  margin: auto;
}
.company-info-block {
  width: 25%;
  display: block;
  margin-right: 100px;
}
.footer-logo {
  width: 100%;
  margin-bottom: 70px;
}
.info-about-company {
  margin-bottom: 40px;
}
.copyrigh {
  font-weight: 500;
  font-size: 14px;
}
.description-company {
  font-weight: 400;
  font-size: 14px;
  color: #9A9A9A;
}
.yandex-rating {
  width: 250px;
  margin-bottom: 40px;
}
.payment-info {
  margin-bottom: 10px;
  font-weight: 600;
  font-size: 14px;
  color: #9A9A9A;
}
.company-contacts-block {
  display: flex;
  margin-bottom: 40px;
}
.number-phone {
  margin-right: 40px;
}
.number {
  font-weight: 600;
  font-size: 32px;
  margin-bottom: 5px;
}
.time-works {
  color: #9A9A9A;
}
.order-button {
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: Montserrat;
  font-weight: 500;
  font-size: 16px;
  padding: 15px 20px 15px 20px;
  box-sizing: border-box;
  border-radius: 10px;
  background-color: #000000;
  color: #ffffff;
  text-decoration: none;
  cursor: pointer;
}
.order-button > span {
  margin-left: 10px;
}
.feedback-messengers {
  display: flex;
  margin-left: 20px;
}
.viber-icon {
  cursor: pointer;
}
.wa-icon {
  margin-left: 20px;
  cursor: pointer;
}
.tg-icon {
  margin-left: 20px;
  cursor: pointer;
}
.navigations-main-block {
  display: flex;
}
.navigation-menu {
  margin-right: 100px;
}
.navigation-title {
  font-weight: 600;
  margin-bottom: 40px;
}
.navigation-link {
  margin-top: 20px;
}
.navigation-link > a {
  color: #000000;
  text-decoration: none;
  cursor: pointer;
}
.feedback-link {
  display: flex;
  align-items: center;
  padding-bottom: 25px;
  margin-top: 25px;
  border-bottom: 2px solid #e6e6e6;
}
.feedback-link > img {
  width: 30px;
  margin-right: 10px;
}
.feedback-link > a {
  font-weight: 600;
  color: #000000;
  text-decoration: none;
  cursor: pointer;
}
.messengers-links {
  display: flex;
  align-items: center;
  margin-top: 25px;
}
.location-link {
  display: flex;
  align-items: center;
  padding-bottom: 25px;
  margin-top: 25px;
  border-bottom: 2px solid #e6e6e6;
}
.location-link > img {
  width: 15px;
  margin-right: 10px;
}
.location-link > span {
  font-weight: 600;
}
.location-button {
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: Montserrat;
  font-weight: 500;
  font-size: 16px;
  padding: 15px 20px 15px 20px;
  margin-top: 20px;
  box-sizing: border-box;
  border-radius: 10px;
  background-color: #F6F6F6;
  color: #000000;
  text-decoration: none;
  cursor: pointer;
}
@media only screen and (max-width : 1536px) {
  .footer-main-container {
    max-width: 1080px;
  }
  .payment-systems > img {
    width: 100%;
  }
  .company-info-block {
    margin-right: 60px;
  }
  .navigation-menu {
    margin-right: 60px;
  }
}
@media only screen and (max-width : 980px) {
  .footer-main-container {
    max-width: 850px;
  }
  .company-info-block {
    display: none;
  }
}
@media only screen and (max-width : 768px) {
  .footer-main-container  {
    max-width: 650px;
    padding: 60px 0 150px 0;
  }
  .number {
    font-size: 25px;
  }
  .order-button > span {
    font-size: 12px;
  }
  .time-works {
    font-size: 12px;
  }
  .wa-icon, .tg-icon {
    margin-left: 10px;
  }
  .navigation-menu {
    margin-right: 40px;
  }
}
@media only screen and (max-width : 320px) {
  .footer-main-container {
    max-width: 320px;
    padding: 60px 0 60px 0;
  }
  .navigations-main-block {
    display: none;
  }
  .company-contacts-block {
    display: block;
  }
  .number-phone {
    margin: 0 0 20px 0;
    text-align: center;
  }
  .contacts-navigations-container {
    margin: auto;
  }
  .callback-button {
    margin-bottom: 20px;
  }
  .feedback-messengers {
    margin: 0;
  }
}
</style>