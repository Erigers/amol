<template>
    <section class="achievement">
        <div class="second-background">
            <div class="first-background">
                <div class="o-container">
                    <img src="~/assets/svg/achievement.svg" alt="achievement-icon">
                    <div class="foot-note">
                        <p>
                            This is my first official idea-to-execution work. <br>
                            Special thanks to my design mentor 7 years ago, <a href="https://dribbble.com/aldohysenaj" target="_blank">Aldo Hysenaj</a> , a.k.a. Doal. <br>
                            You can easily find him, he’s famous now. <br>
                            This is for always doing more than we are expected of.
                        </p>
                    </div>
                    <div class="doal">
                        <img src="/doal.png" alt="doal-image">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
.achievement {
    background: $color-blue;
    padding: 0 5px 50px 5px;
    .second-background {
        background: url(~/assets/svg/footer-second-background.svg);
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        width: calc(100% - 40px);
        position: relative;
        .first-background {
            background: url(~/assets/svg/footer-first-background.svg);
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
            width: 100%;
            margin-left: 20px;
            position: relative;
            top: 20px;
            max-width: 1388px;
            .o-container {
                display: flex;
                flex-direction: column;
                justify-content: center;
                @include mq($from: desktop) {
                    flex-direction: row;
                    justify-content: space-between;
                }
                img[alt="achievement-icon"] {
                    width: 68px;
                    margin: auto;
                }
                .foot-note p {
                    color: $color-white;
                    font-size: 16px;
                    @include mq($from: desktop) {
                        width: 70%;
                        font-size: 22px;
                    }
                    a {
                        color: $color-red;
                    }
                }
                .doal {
                    display: flex;
                    justify-content: center;
                    img {
                        width: 200px;
                        margin: auto;
                    }
                }
            }
        }
    }
}
</style>
