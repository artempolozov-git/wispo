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
</style>