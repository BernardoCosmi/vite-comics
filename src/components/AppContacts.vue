<script>
// import

export default {
  name: "AppContacts",
};
</script>

<template>
  <div class="container">
    <div class="contacts-container">

      <div class="column-container">
        <div class="column one">
            <h3>dc comics</h3>
            <ul>
                <a>characters</a>
                <a>comics</a>
                <a>movies</a>
                <a>TV</a>
                <a>games</a>
                <a>videos</a>
                <a>news</a>
            </ul>
            <h3>shop</h3>
            <ul>
                <a>shop DC</a>
                <a>shop DC collectibles</a>
            </ul>
        </div>
        <div class="column two">
            <h3>DC</h3>
            <ul>
                <li><a>terms of use</a></li>
                <li><a>privacy policy(new)</a></li>
                <li><a>ad choices</a></li>
                <li><a>advertising</a></li>
                <li><a>jobs</a></li>
                <li><a>subscription</a></li>
                <li><a>talent workshops</a></li>
                <li><a>CPSC certificates</a></li>
                <li><a>ratings</a></li>
                <li><a>shop help</a></li>
                <li><a>contact us</a></li>
            </ul>
        </div>
        <div class="column three">
            <h3>sites</h3>
            <ul>
                <li><a href="">DC</a></li>
                <li><a href="">MAD magazine</a></li>
                <li><a href="">DC kids</a></li>
                <li><a href="">DC universe</a></li>
                <li><a href="">DC power visa</a></li>
            </ul>
        </div>
      </div>

      <figure>
        <img src="../assets/images/dc-logo-bg.png" alt="logo grande">
      </figure>  

    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.container{
  width: 100%;
  height: 350px;
  background-image: url('../assets/images/footer-bg.jpg');
  display: flex;
  align-items: center;
  justify-content: space-between;
  overflow: hidden;
}
.contacts-container{
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.column-container{
    display: flex;
    gap: 20px;
}
h3{
    color: white;
    text-transform: uppercase;
    margin-bottom: 0;
}
ul{
    display: flex;
    flex-direction: column;
    list-style-type: none;
    padding: 0;
    text-align: left;
}
a{
    text-decoration: none;
    text-transform: capitalize;
    font-weight: normal;
    font-size: smaller;
    color: grey;
}

</style>
