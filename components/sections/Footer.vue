<template>
    <footer>
        <div class="o-container">
            <h4>made with</h4>
            <img src="/heart.png" alt="heart-icon">
            <h4>by Erigers Mamoci</h4>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
footer {
    background: url(~/assets/svg/footer-background.svg);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    width: 100%;
    padding: 30px 0 20px 0;
    .o-container {
        display: flex;
        // justify-content: flex-start;
    }
    h4 {
        color: $color-white;
        font-family: $font-header;
    }
    img {
        width: 44px;
        height: 44px;
        margin-top: 18px;
    }
}
</style>
