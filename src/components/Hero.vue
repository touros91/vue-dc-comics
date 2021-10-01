<template>
    <section>
        <div class="hero">
            <img :src="heroSrc" :alt="heroAlt">
        </div>
    </section>

</template>

<script>
export default {
    name: 'Hero',
    props: ['heroSrc', 'heroAlt']
}
</script>

<style lang="scss" scoped>
    .hero {
        width: 100%;
        height: 270px;
        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: 0px 0px;
        }
    }
</style>