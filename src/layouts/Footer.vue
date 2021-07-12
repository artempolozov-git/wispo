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
          <div class="catalog-nav">
            <div class="catalog-title">Каталог</div>
            <div class="catalog-links" ><a href="#">Смартфоны</a></div>
            <div class="catalog-links" ><a href="#">Планшеты и компьюетры</a></div>
            <div class="catalog-links" ><a href="#">Умные часы и браслеты</a></div>
            <div class="catalog-links" ><a href="#">Гаджеты</a></div>
            <div class="catalog-links" ><a href="#">Аудиотехника</a></div>
            <div class="catalog-links" ><a href="#">Другое</a></div>
            <div class="catalog-links" ><a href="#">Топ гаджеты</a></div>
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

}
.catalog-title {
  font-weight: 600;
  margin-bottom: 40px;
}
.catalog-links {
  margin-top: 20px;
}
.catalog-links > a {
  color: #000000;
  text-decoration: none;
  cursor: pointer;
}
</style>