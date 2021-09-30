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
        width: calc(100% / 6 - 10px);
        margin: 0 5px;
        .serie-img {
            width: 100%;
            img{
                width: 100%;
            }   
        }
        .serie-title {
            margin: 10px 0 40px 0;
            font-size: 15px;  
        }
        a {
            color: white;
            text-decoration: none;
        }
    }
</style>