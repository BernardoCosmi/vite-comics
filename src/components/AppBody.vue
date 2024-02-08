<script>
import ComicsCards from "./ComicsCards.vue";
import comicsData from "../../dc-comics.json";

export default {
  components: {
    ComicsCards
  },
  data() {
    return {
      comics: comicsData
    };
  }
};
</script>

<template>
  <div class="container">
    <div class="jumbotron">

    </div>
    <span>
      
    </span>
    <div class="cards-container">
      <ComicsCards :comics="comics" />
    </div>
  </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.container{
    background: #1C1C1C;
}
.cards-container {
  width: 80%;
  margin: 0 auto;
  padding: 20px;

}
</style>
