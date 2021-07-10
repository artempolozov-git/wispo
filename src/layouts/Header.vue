<template>
  <div class="header">
    <header-navigation></header-navigation>
    <header-panel></header-panel>
    <header-catalog></header-catalog>
  </div>
</template>

<script>
    import HeaderNavigation from "@/components/HeaderNavigation";
    import HeaderPanel from "@/components/HeaderPanel";
    import HeaderCatalog from "@/components/HeaderCatalog";
    export default {
        name: "Header",
        components: {HeaderCatalog, HeaderPanel, HeaderNavigation}
    }
</script>

<style scoped>
.header {
  height: auto;
  background-color: #ffffff;
}
</style>