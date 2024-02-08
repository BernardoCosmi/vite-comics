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
   

    <span class="current-series">
      current series
    </span>



    <div class="cards-container">
      <ComicsCards :comics="comics" />
      <span>
        load more
      </span>
    </div>
  </div>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.container{
    background: #1C1C1C;
}
.jumbotron{
  background-image: url(../assets/images/jumbotron.jpg);
  background-size: 100%;
  width: 100%;
  height: 350px;
}
.current-series{
  color: white;
  background-color: #0282F9;
  font-size: x-large;
  font-weight: bold;
  text-transform: uppercase;
  padding: 10px 40px;
  position: absolute;
  left: 10%;
  top: 425px;
}
.cards-container {
  width: 80%;
  margin: 0 auto;
  padding: 20px;
  display: flex;
  flex-direction: column;
  span{
    margin: 0 auto;
    color: white;
    font-weight: bold;
    text-transform: uppercase;
    background-color: #0282F9 ;
    padding: 10px 40px;
  }
}
</style>
