<script>
import AppHeader from "./components/AppHeader.vue"
import AppBody from "./components/AppBody.vue"
import AppLinks from "./components/AppLinks.vue"
import AppContacts from "./components/AppContacts.vue"
import AppFooter from "./components/AppFooter.vue"

export default {
  components: {
    AppHeader,
    AppBody,
    AppLinks,
    AppContacts,
    AppFooter,
  },
};
</script>

<template>
    <AppHeader/>
    <AppBody/>
    <AppLinks/>
    <AppContacts/>
</template>

<style lang="scss">
@use "./styles/general.scss";

body{
    margin:0;
}
</style>
