<script>
// import

export default {
  name: "AppBody",
};
</script>

<template>
  <div class="container">
    <div>
        <h1> &rarr; Content goes here &larr;</h1>
    </div>

  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.container{
  width: 100vw;
  background: #1C1C1C;
  div{
    width: 80%;
    margin: 10px auto;
    height: 150px;
    text-align: start;
    display: flex;
    align-items: center;
  }
}
h1{
  color: white;
}
</style>
