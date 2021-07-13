<template>
  <div class="home">
    <device-category></device-category>
    <device-characteristics></device-characteristics>
  </div>
</template>

<script>
    import DeviceCategory from "@/components/DeviceCategory";
    import DeviceCharacteristics from "@/components/DeviceCharacteristics";
    export default {
        name: "Home",
        components: {DeviceCharacteristics, DeviceCategory},
    }
</script>

<style scoped>
.home {
  background-color: white;
  max-width: 1520px;
  padding: 50px 30px;
  box-sizing: border-box;
  margin: 30px auto 50px;
  border-radius: 10px;
  box-shadow: 0px 12px 10px -2px rgba(230, 230, 230, 0.8);
}
@media only screen and (max-width : 1536px) {
  .home {
    max-width: 1080px;
  }
}
@media only screen and (max-width : 980px) {
  .home {
    max-width: 850px;
  }
}
@media only screen and (max-width : 768px) {
  .home {
    max-width: 650px;
  }
}
@media only screen and (max-width : 701px) {
  .home  {
    max-width: 320px;
  }
}
</style>