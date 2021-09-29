<template>
    <div class="second-section">
        <div class="container">
            <div class="icons-container">
                <ul>
                    <li v-for="(icon, index) in icons" :key="index">
                        <div class="icon">
                            <div class="icon-img">
                                <img :src="`images/` + icon.src">
                            </div>  
                            <span>{{icon.name}}</span>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ComicsSecondSection',
    data(){
        return {
            icons: [
                {
                    name: 'DIGITAL COMICS',
                    src: 'buy-comics-digital-comics.png'
                },
                {
                    name: 'DC MERCHANDISE',
                    src: 'buy-comics-merchandise.png'
                },
                {
                    name: 'SUBSCRIPTIONS',
                    src: 'buy-comics-subscriptions.png'
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    src: 'buy-comics-shop-locator.png'
                },
                {
                    name: 'DC POWER VISA',
                    src: 'buy-dc-power-visa.svg'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .second-section {
        background-color: #0282F9;
        padding: 20px;
        .icons-container {
            ul {
                display: flex;
                justify-content: space-between;
                li {
                    align-self: center;
                    list-style: none;
                .icon {
                    display: flex;
                    .icon-img {
                        max-width: 40px;
                        align-self: center;
                        img{
                            width: 100%;
                        }
                    }  
                    span {
                        font-size: 14px;
                        align-self: center;
                        color: white;
                        margin-left: 10px;
                    }
                }

                }
            }
        }
    }
</style>