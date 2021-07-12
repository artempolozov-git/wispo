<template>
  <div class="header">
    <header-navigation></header-navigation>
    <header-panel></header-panel>
    <header-catalog></header-catalog>
    <bread-crumbs></bread-crumbs>
  </div>
</template>

<script>
    import HeaderNavigation from "@/components/HeaderNavigation";
    import HeaderPanel from "@/components/HeaderPanel";
    import HeaderCatalog from "@/components/HeaderCatalog";
    import BreadCrumbs from "@/components/BreadCrumbs";
    export default {
        name: "Header",
        components: {BreadCrumbs, HeaderCatalog, HeaderPanel, HeaderNavigation}
    }
</script>

<style scoped>
.header {
  height: auto;
  background-color: #ffffff;
}
</style>