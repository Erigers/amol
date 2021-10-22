<template>
    <section class="background-story">
        <div class="o-container">
            <h2>A short background story...</h2>
            <div class="o-row">
                <div class="column-not-center">
                    <img src="/erigers.png" alt="erigers-mamoci-profile-pic">
                </div>
                <div class="column-center">
                    <p>&nbsp;&nbsp;My name is Erigers, am a programmer @FIZ, an entrepreneur in spirit from Albania and I only did this project because I am grateful</p>
                </div>
                <div class="column-not-center" />
            </div>
            <div class="o-row">
                <div class="column-not-center" />
                <div class="column-center">
                    <p>to my German teacher Angela & her newly-wed husband Franzjörg invited me to their circle celebrating their union.</p>
                </div>
                <div class="column-not-center" />
            </div>
            <div class="o-row">
                <div class="column-center">
                    <img src="/franzjorg-wed.gif" alt="franzjorg-wed">
                    <img src="/angela-wed.gif" alt="angela-wed">
                    <img src="~/assets/svg/platform.svg" alt="wed-platform">
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
h2 {
    width: 100%;
    text-align: center;
}
p {
    @include mq($from: desktop) {
        font-size: 32px;
    }
}
</style>
