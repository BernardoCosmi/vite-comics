<script>
export default {
  props: {
    comics: {
      type: Array,
      required: true
    }
  }
};
</script>

<template>
  <div>
    <div class="comics-list">
      <div v-for="(comic, index) in comics" :key="index" class="comic-card">
        <img :src="comic.thumb" :alt="comic.series" class="comic-thumb">
        <div class="comic-details">
          <h3>{{ comic.series }}</h3>
          <p>Type: {{ comic.type }}</p>
          <p>Price: {{ comic.price }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.comics-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
}

.comic-card {
  border: 1px solid #ccc;
  border-radius: 5px;
  padding: 10px;
}

.comic-thumb {
  width: 100px;
  height: auto;
  margin-right: 10px;
}
</style>