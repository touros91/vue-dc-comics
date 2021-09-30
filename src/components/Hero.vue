<template>
    <section>
        <div class="hero">
            <img src="images/jumbotron.jpg" alt="Hero Image">
        </div>
    </section>

</template>

<script>
export default {
    name: 'Hero'
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
            object-position: 0px 10px;
        }
    }
</style>