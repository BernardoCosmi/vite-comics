<script>
export default {
  name: "AppHeader",
};

</script>

<template>
  <div class="container">
    <!-- LOGO -->
    <div>
      <img src="../assets/images/dc-logo.png" alt="Logo Dc Comix">
    </div>

    <!-- Menu -->
    <div>
      <ul>
        <li>
          <span>characters</span>
        </li>
        <li>
          <span>comics</span>
        </li>
        <li>
          <span>movies</span>
        </li>
        <li>
          <span>tv</span>
        </li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
      </ul>
    </div>
    
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.container{
  display: flex;
  width: 80vw;
  margin: auto;
  justify-content: space-between;
}
ul{
  list-style-type: none;
  display: flex;
}

</style>
