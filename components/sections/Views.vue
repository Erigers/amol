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
    .o-row {
        align-items: baseline;
        .o-column-not-center {
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
                    left: 60px;
                    top: 30px;
                    font-family: $font-header;
                    color: $color-white;
                    font-size: 52px;
                }
            }
        }
    }
}
</style>
