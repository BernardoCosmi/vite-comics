<script>
import AppHeader from "./components/AppHeader.vue"
import AppBody from "./components/AppBody.vue"
import AppLinks from "./components/AppLinks.vue"
import AppFooter from "./components/AppFooter.vue"

export default {
  components: {
    AppHeader,
    AppBody,
    AppLinks,
    AppFooter,
  },
};
</script>

<template>
    <AppHeader/>
    <AppBody/>
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
