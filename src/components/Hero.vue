<template>
    <section>
        <div class="hero">
            <img :src="jumbotron" alt="Hero Image">
        </div>
    </section>

</template>

<script>
export default {
    name: 'Hero',
    props: ['jumbotron']
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