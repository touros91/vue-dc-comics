<template>
    <div class="serie">
        <a href="#">
            <div class="serie-img">
                <img :src="card.thumb" :alt="card.series">
            </div>
        </a>    
        <a href="#">
            <div class="serie-title">{{card.series.toUpperCase()}}</div>
        </a>
    </div>
</template>

<script>
export default {
    name: 'Serie',
    props: ['card']
}
</script>

<style lang="scss" scoped>
    .serie {
        width: calc(100% / 6 - 30px);
        margin: 0 15px;
        .serie-img {
            width: 100%;
            img{
                width: 100%;
            }   
        }
        .serie-title {
            margin: 10px 0 40px 0;
            font-size: 13px; 
        }
        a {
            color: white;
            text-decoration: none;
        }
    }
</style>