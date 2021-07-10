<template>
  <div id="app">
    <router-view name="header"></router-view>
    <div id="app-content">
      <transition name="app-router-fade" mode="out-in">
        <router-view :key="defaultViewKey"></router-view>
      </transition>
    </div>
    <router-view name="footer"></router-view>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {

  },
  computed: {
      defaultViewKey: function () {
          return this.$route.name;
      }
  }
}
</script>

<style>
  html, body {
    height: 100%;
  }
  body {
    margin: initial;
    font-family: Montserrat;
    font-size: 14px;
    font-weight: 400;
    background-color: #F6F6F6;
  }
  #app {
    display: flex;
    flex-direction: column;
    min-height: 100%;
    background-color: #F6F6F6;
  }
  @font-face {
    font-family: Montserrat;
    src: url('./assets/Montserrat-Regular.ttf');
    font-weight: 400;
  }
  @font-face {
    font-family: Montserrat;
    src: url('./assets/Montserrat-Medium.ttf');
    font-weight: 500;
  }
  @font-face {
    font-family: Montserrat;
    src: url('./assets/Montserrat-SemiBold.ttf');
    font-weight: 600;
  }
  #app-content {
    flex: 1 0 auto;
    max-width: 1920px;
    align-self: center;
    width: -webkit-fill-available;
  }
</style>
