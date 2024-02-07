<script>
// import

export default {
  name: "AppLinks",
  data(){
    return{
      ArrayUsefulLinks:[
        {
          imageName: 'buy-comics-digital-comics.png',
          title: 'digital comics'
        },
        {
          imageName: 'buy-comics-merchandise.png',
          title: 'dc merchandise'
        },
        {
          imageName: 'buy-comics-subscriptions.png',
          title: 'subscription'
        },
        {
          imageName: 'buy-comics-shop-locator.png',
          title: 'comic shop locator'
        },
        {
          imageName: 'buy-dc-power-visa.png',
          title: 'dc power visa'
        },
        
      ]
    };
  },
  methods: {
  getImagePath: function(img) {
    return new URL(`../assets/images/${img}`, import.meta.url).pathname;
  }
  }
};
</script>

<template>
  <div class="container">
    <div class="link-container">
      <div class="link-card" v-for="(element, index) in ArrayUsefulLinks">
        <img :src="getImagePath(element.imageName)" alt="logo">
        <span>{{ element.title }}</span>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.container{
  width: 100%;
  background: #0282f9;
  color: white;
}
.link-container{
  width: 80%;
  min-height: 130px;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: space-around;
}
.link-card{
    display: flex;
    align-items: center;
    gap: 10px;
    min-width: 50px;

    img{
      max-height: 60px;
      max-width: 60px;
    }
    span{
      text-transform: uppercase;
      font-size: smaller;
      white-space: nowrap;
    }
}
 
</style>
