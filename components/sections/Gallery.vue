<template>
    <section class="gallery">
        <h2>Pictures from the wedding</h2>
        <div class="gallery-holder">
            <div class="o-container">
                <!-- <div class="left-arrow arrow" /> -->
                <div class="slider">
                    <div class="slide">
                        <img src="/gallery/photo-1.jpg" alt="photo-1">
                    </div>
                    <div class="slide">
                        <img src="/gallery/photo-2.jpg" alt="photo-2">
                    </div>
                    <div class="slide">
                        <img src="/gallery/photo-3.jpg" alt="photo-3">
                    </div>
                </div>
                <!-- <div class="right-arrow arrow" /> -->
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
.gallery-holder {
    background: $color-primary;
    padding: 40px 0;
    .o-container {
        background: url(~/assets/svg/background-pink.svg);
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        // height: 431px;
        padding: 40px 0;
        .arrow {
            width: 20px;
            height: 20px;
        }
        .slider {
            width: 100%;
            @include mq($from: desktop) {
                display: flex;
                justify-content: space-between;
            }
            .slide {
                width: 90%;
                margin: auto;
                @include mq($from: desktop) {
                    width: calc(100% / 3 - 20px);
                }
                img {
                    width: 100%;
                    border-radius: 10px;
                    overflow: hidden;
                }
            }
        }
    }
}
</style>
