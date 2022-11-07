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
            return new URL(`./assets/img/${this.imgNameVite}`, import.meta,url).href;
        }
    }
}
</script>
<template>
    <div class="banner">
        <img :src="getImagePathVue()" alt="">

    </div>
</template>
<style scoped>
.banner {
    width: 100%;
    height: 30vh;
}
.banner img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
</style>