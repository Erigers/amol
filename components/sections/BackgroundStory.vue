<template>
    <section class="background-story">
        <div class="o-container">
            <h2>A short background story...</h2>
            <div class="o-row">
                <div class="o-column-not-center">
                    <img src="/erigers.png" alt="erigers-mamoci-profile-pic">
                </div>
                <div class="o-column-center">
                    <p>&nbsp;&nbsp;My name is Erigers, a programmer @FIZ, an entrepreneur in spirit from Albania and I only did this project because I am grateful</p>
                </div>
                <div class="o-column-not-center">
                    <img src="/Albanian-Flag.png" alt="albanian-flag">
                </div>
            </div>
            <div class="o-row">
                <div class="o-column-not-center">
                    <img src="/German-Flag.png" alt="german-flag">
                </div>
                <div class="o-column-center">
                    <p>to my German teacher Angela & her newly-wed husband Franzjörg invited me to their circle celebrating their union.</p>
                </div>
                <div class="o-column-not-center" />
            </div>
            <div class="o-row">
                <div class="o-column-not-center" />
                <div class="o-column-center">
                    <div class="marriage-platform">
                        <img src="/franzjorg-wed.gif" alt="franzjorg-wed">
                        <img src="/angela-wed.gif" alt="angela-wed">
                        <img src="~/assets/svg/platform.svg" alt="wed-platform">
                    </div>
                </div>
                <div class="o-column-not-center" />
            </div>
            <div class="o-row">
                <div class="o-column-not-center" />
                <div class="o-column-center">
                    <p>&nbsp;&nbsp;&nbsp;&nbsp;A while back, Angela expressed that she missed the map at her office where she had a pin for every nationality of her colleagues due to Covid-19 work from home restrictions</p>
                </div>
                <div class="o-column-not-center" />
            </div>
            <div class="o-row gift-row">
                <div class="o-column-not-center" />
                <div class="o-column-center">
                    <p class="ellipsis">...</p>
                </div>
                <div class="o-column-not-center">
                    <img src="~/assets/svg/gift.svg" alt="gift-svg">
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
.background-story {
    margin-top: 0px;
    @media screen and (max-height: 700px) {
      margin-top: 200px;
    }
}
img[alt="erigers-mamoci-profile-pic"] {
    width: 100px;
    @include mq($from: desktop) {
        width: 150px;
        margin-top: -100px;
    }
}
img[alt="albanian-flag"] {
    width: 75px;
    height: 75px;
    @include mq($from: desktop) {
        width: 100px;
        height: 100px;
        margin-top: 100px;
        margin-right: 20px;
    }
}
img[alt="german-flag"] {
    max-width: 65px;
    width: 100%;
    height: auto;
    @include mq($from: desktop) {
        width: 90px;
        margin-top: 120px;
        margin-left: 40px;
    }
}
.o-row:nth-child(2) {
    .o-column-not-center:nth-child(3) {
        display: flex;
        justify-content: flex-end;
    }
}
// third row
img[alt="wed-platform"] {
    width: 200px;
    @include mq($from: phablet) {
        width: 300px;
    }
}
img[alt="franzjorg-wed"], img[alt="angela-wed"] {
    position: relative;
    width: 80px;
    margin-bottom: -40px;
    border-radius: 100px;
    overflow: hidden;
    @include mq($from: phablet) {
        width: 140px;
    }
}
img[alt="franzjorg-wed"] {
    margin-left: 30px;
    @include mq($from: phablet) {
        margin-left: 30px;
        margin-right: -30px;
    }
}
.marriage-platform {
    position: relative;
    width: 200px;
    margin: 50px auto;
    @include mq($from: phablet) {
        width: 300px;
    }
}
// fourth row
.gift-row {
    position: relative;
    p {
        font-size: 70px;
        font-family: $font-header;
        width: 100%;
        text-align: center;
        margin: 0;
        @include mq($from: phablet) {
            font-size: 100px;
        }
    }
    .o-column-not-center {
        display: flex;
        justify-content: flex-end;
        img[alt="gift-svg"] {
            width: 85px;
            margin-right: 40px;
            margin-top: -60px;
            @include mq($from: phablet) {
                margin-right: 40px;
                margin-top: 40px;
            }
        }
    }
}
</style>
