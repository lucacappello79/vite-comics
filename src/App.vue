<script>
import AppHeader from "./components/AppHeader.vue"
import AppMain from "./components/AppMain.vue"
import AppFooter from "./components/AppFooter.vue"
import AppFeatured from "./components/AppFeatured.vue"
import AppSocial from "./components/AppSocial.vue"


export default {
  data() {
    return {
      viewTitle: true,
    };
  },

  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppFeatured,
    AppSocial,
  },

};
</script>

<template>
  <AppHeader></AppHeader>
  <AppMain></AppMain>
  <AppFeatured></AppFeatured>
  <AppFooter></AppFooter>
  <AppSocial></AppSocial>
</template>

<style lang="scss">
ul {
  list-style-type: none;
}

a {
  text-decoration: none;

  &:hover {
    color: blue;
  }
}
</style>


