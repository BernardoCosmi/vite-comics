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
                <div class="comic-thumb">
                    <figure class="comic-thumb">
                        <img :src="comic.thumb" :alt="comic.series">
                    </figure>
                    <h4>{{ comic.series }}</h4>
                </div>

                <div class="comic-details">
                    <p>{{ comic.type }}</p>
                    <p>{{ comic.price }}</p>
                </div>

            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.comics-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    row-gap: 50px;
    margin: 20px 0;
}
.comic-card {
    padding: 2px;
    width: calc(90%/6);
    display: flex;
    flex-direction: column;
    row-gap: 5px;
    &:hover{
        border: 2px solid white;
        scale: 1.15;
    }
    &:hover p{
        color: white;
    }
}
.comic-thumb {
    figure{
        width: 100%;
        aspect-ratio: 1 / 1;
        overflow: hidden;
        
        img {
            width: 100%;
        }
    }
}
h4 {
    text-transform: uppercase;
    color: white;
    text-align: center;
    margin-top: 10px;
}
.comic-details {
    text-align: center;
    color: white;
    margin-top: 5px;
    display: flex;
    justify-content: space-evenly;
    p {
        color: grey;
        text-transform: capitalize;
    }
}</style>