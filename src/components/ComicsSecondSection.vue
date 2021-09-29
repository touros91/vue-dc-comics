<template>
    <div class="second-section">
        <div class="container">
            <div class="icons-container">
                <div class="icon">
                    <div class="icon-img">
                        <img src="@/assets/images/buy-comics-digital-comics.png" alt="Digital Comics">
                    </div>
                    <span>DIGITAL COMICS</span>
                </div>
                <div class="icon">
                    <div class="icon-img">
                        <img src="@/assets/images/buy-comics-merchandise.png" alt="Digital Comics">
                    </div>
                    <span>DC MERCHANDISE</span>
                </div>
                <div class="icon">
                    <div class="icon-img">
                        <img src="@/assets/images/buy-comics-subscriptions.png" alt="Digital Comics">
                    </div>
                    <span>SUBSCRIPTIONS</span>
                </div>
                <div class="icon">
                    <div class="icon-img">
                        <img src="@/assets/images/buy-comics-shop-locator.png" alt="Digital Comics">
                    </div>
                    <span>COMIC SHOP LOCATOR</span>
                </div>
                <div class="icon">
                    <div class="icon-img">
                        <img src="@/assets/images/buy-dc-power-visa.svg" alt="Digital Comics">
                    </div>
                    <span>DC POWER VISA</span>
                </div>
                
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: 'ComicsSecondSection'
}
</script>

<style lang="scss" scoped>
    .second-section {
        background-color: #0282F9;
        padding: 20px;
        .icons-container {
            display: flex;
            justify-content: space-between;
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
</style>