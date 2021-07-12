<template>
  <div class="crumbs-wrapper">
    <div class="crumbs-container">
      <span class="bread-crumbs">Главная &nbsp; / &nbsp; Сравнение товаров</span>
      <h1 class="bread-title">Сравнение товаров</h1>
    </div>
  </div>
</template>

<script>
    export default {
        name: "BreadCrumbs"
    }
</script>

<style scoped>
.crumbs-wrapper {
  box-shadow: 0px 10px 5px -4px rgba(230, 230, 230, 0.5) inset;
}
.crumbs-container {
  display: block;
  box-sizing: border-box;
  max-width: 1520px;
  width: 100%;
  padding: 40px 0 40px 0;
  margin: auto;
}
.bread-crumbs {
  font-weight: 500;
  color: #9A9A9A;
  cursor: pointer;
}
.bread-title {
  margin-bottom: 0;
  font-size: 32px;
}
</style>