<script>
// import

export default {
  name: "AppFooter",
};
</script>

<template>
  <div class="bg-container">

    <div class="footer-container">

      <span>
        sign-up now!
      </span>

      <div class="icon-container">
        <span>follow us</span>
        <img src="../assets/images/footer-facebook.png" alt="">
        <img src="../assets/images/footer-twitter.png" alt="">
        <img src="../assets/images/footer-youtube.png" alt="">
        <img src="../assets/images/footer-pinterest.png" alt="">
        <img src="../assets/images/footer-periscope.png" alt="">
      </div>

    </div>

  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.bg-container {
  background-color: #303030;
  width: 100%;
  height: 100px;
}

.footer-container {
  width: 80%;
  height: 100px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

span {
  text-transform: uppercase;
  background-color: #303030;
  border: 2px solid #0282F9;
  color: white;
  width: 150px;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.icon-container {
  display: flex;
  gap: 20px;
  span {
    border: none;
    color: #0282F9;
    font-weight:800;
    width: auto;
    height: auto;
  }
}</style>
