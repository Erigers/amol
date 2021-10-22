<template>
    <section class="views">
        <div class="o-container">
            <h2>This many people have seen you happily wed</h2>
            <div class="o-row">
                <div class="o-column-not-center">
                    <img src="~/assets/svg/candles/left-column.svg" alt="left-candle">
                </div>
                <div class="o-column-center">
                    <div class="candle">
                        <div class="counter">1</div>
                        <img src="~/assets/svg/candles/first-counter.svg" alt="first-counter-candle">
                    </div>
                    <div class="candle">
                        <div class="counter">1</div>
                        <img src="~/assets/svg/candles/second-counter.svg" alt="second-counter-candle">
                    </div>
                    <div class="candle">
                        <div class="counter">1</div>
                        <img src="~/assets/svg/candles/third-counter.svg" alt="third-counter-candle">
                    </div>
                </div>
                <div class="o-column-not-center">
                    <img src="~/assets/svg/candles/right-column.svg" alt="right-candle">
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
.views {
    margin-top: 50px;
    padding: 50px 0 100px 0;
    .o-row {
        position: relative;
        align-items: baseline;
        padding-top: 100px;
        @include mq($from: desktop) {
            padding-top: 0;
        }
        .o-column-not-center {
            position: relative;
            width: 40px;
            @include mq($from: desktop) {
                width: 150px;
            }
            &:nth-child(1) {
                order: 1;
                position: absolute;
                top: 0;
                left: 0;
                @include mq($from: desktop) {
                    position: static;
                }
            }
            &:nth-child(3) {
                position: absolute;
                top: 0;
                right: 0;
                order: 2;
                @include mq($from: desktop) {
                    order: 3;
                    position: static;
                }
            }
            img {
                width: 40px;
                @include mq($from: desktop) {
                    width: 100%;
                }
            }
        }
        .o-column-center {
            display: flex;
            justify-content: space-evenly;
            align-items: baseline;
            order: 3;
            @include mq($from: desktop) { order: 2 }
            .candle {
                position: relative;
                width: 80px;
                @include mq($from: desktop) {
                    width: 140px;
                }
                img {
                    width: 100%;
                }
                .counter {
                    position: absolute;
                    color: $color-white;
                    font-family: $font-header;
                    left: 40px;
                    top: 20px;
                    font-size: 32px;
                    @include mq($from: desktop) {
                        left: 60px;
                        top: 30px;
                        font-size: 52px;
                    }
                }
            }
        }
    }
}
</style>
