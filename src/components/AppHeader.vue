<script>
export default {
  name: "AppHeader",
  data() {
    return {
      ArrayLinksMenu: [
        {
          title: 'characters',
          link: '#',
          active: false
        },
        {
          title: 'comics',
          link: '#',
          active: false
        },
        {
          title: 'movies',
          link: '#',
          active: false
        },
        {
          title: 'tv',
          link: '#',
          active: false
        },
        {
          title: 'games',
          link: '#',
          active: false
        },
        {
          title: 'collectibles',
          link: '#',
          active: false
        },
        {
          title: 'videos',
          link: '#',
          active: false
        },
        {
          title: 'fans',
          link: '#',
          active: false
        },
        {
          title: 'news',
          link: '#',
          active: false
        },
        {
          title: 'shop',
          link: '#',
          active: false
        },
      ]
    }
  }
};


</script>

<template>
  <div class="container">
    <!-- LOGO -->
    <div>
      <img src="../assets/images/dc-logo.png" alt="Logo Dc Comix">
    </div>

    <!-- Menu -->
    <div class="menu-container">
      <ul>
        <li v-for="(element, index) in ArrayLinksMenu">
          <a :href="element.link">{{ element.title }}</a>
        </li>
      </ul>
    </div>

  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.container {
  display: flex;
  margin: 0 auto;
  width: 80vw;
  justify-content: space-between;
  align-items: center;
}

img {
  width: 90px;
  height: 90px;
}

ul {
  list-style-type: none;
  display: flex;
  column-gap: 20px;
  height: 100px;
  margin: 0;    


  li {
    text-transform: uppercase;
    font-size: small;
    font-size: 900;
    height: 100%;
    display: flex;
    align-items: center;

    &:hover{
      border-bottom: 5px solid #0282F9;
    }

    a {
      text-decoration: none;
      color: black;
      margin: 0;
      padding: 0;
    }
  }
}</style>
