<script>
export default {
    name: "AppBanner",
    data() {
        return {
            title: "Banner title",
            imgName: "fondo-pag-speciali.jpg",
            // secondImg: "..."
        }
    },
    methods: {
        getImagePath(imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }
}
</script>

<template>
    <section>
        <h2>Titolo del banner</h2>
        <img :src="getImagePath(`../assets/img/${this.imgName}`)" alt="">
        <!-- <img :src="getImagePath(`../assets/img/${this.secondImg}`)" alt=""> -->
        <!-- <img src="/img/fondo-pag-speciali.jpg" alt=""> -->
    </section>
</template>

<style scoped>
img {
    max-width: 100%;
}

h2 {
    color: green;
}
</style>