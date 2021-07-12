<template>
  <div class="feedback-section">
    <div class="feedback-main-container">
      <div class="question-block">
        <div class="question-icon"><img src="@/assets/icons/question-cloud.svg"></div>
        <div class="question-stroke">
          <div class="question-title">Не нашли то что искали?</div>
          <div class="question-description">Остались вопросы? Ответим не стесняясь!</div>
        </div>
      </div>
      <div class="buttons-block">
        <a class="answer-button" href="#"><span>Ответы на популярные вопросы</span></a>
        <a class="feedback-button" href="#"><img src="@/assets/icons/callback-cloud.svg"></a>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "FooterFeedbackSection"
    }
</script>

<style scoped>
.feedback-section {
  border-bottom: 1px solid #e6e6e6;
}
.feedback-main-container {
  display: flex;
  align-items: center;
  box-sizing: border-box;
  padding: 25px 0 25px 0;
  max-width: 1520px;
  margin: auto;
  height: 160px;
}
.question-block {
  display: flex;
  align-items: center;
}
.question-icon {
  margin-right: 40px;
}
.question-title {
  font-weight: 600;
  font-size: 32px;
}
.question-description {
  font-weight: 500;
  font-size: 14px;
}
.buttons-block {
  display: flex;
  margin-left: auto;
}
.answer-button {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 70px;
  border: 3px solid #000000;
  padding: 25px 60px 25px 60px;
  margin-right: 20px;
  box-sizing: border-box;
  border-radius: 10px;
  text-decoration: none;
}
.answer-button > span {
  font-family: Montserrat;
  font-weight: 500;
  font-size: 16px;
  color: #000000;
}
.feedback-button > img {
  width: 320px;
}
</style>