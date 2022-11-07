<script>
export default {
    data() {
        return {
            imgNameVue: `Vue.png`,
            imgNameVite: `Vite.jpg`
        }
    },
    methods: {
        getImagePathVue() {
            return new URL(`../assets/img/${this.imgNameVue}`, import.meta.url).href;
        },
        getImagePathVite() {
            return new URL(`../assets/img/${this.imgNameVite}`, import.meta.url).href;
        }
    }
}
</script>
<template>
    <div class="banner">
        <img :src="getImagePathVue()" alt="">
        <h1> + </h1>
        <img :src="getImagePathVite()" alt="">
    </div>
</template>
<style scoped>
.banner {
    width: 100%;
    height: 30vh;

    display: flex;
    align-items: center;
}
.banner img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
</style>