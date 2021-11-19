<template>
  <div class="landing">
    <Header />
    <Sections-Welcome />
    <Sections-Background-Story />
    <Sections-Gallery />
    <Sections-Views />
    <!-- <Sections-Achievement /> -->
    <Sections-Footer />
    <!-- <section class="open-source-section">
      <h2>Open Source</h2>
      <p>Remember, this is a free for everyone project and open source.</p>
      <ul>
        <li>I am using Vercel’s serverless service to keep the project accessible to you. </li>
        <li>Time spent on the project is a gift for my teacher, Angela.</li>
        <li>I am going to maintain this project, bring new updates if it can serve for more good purposes.</li>
        <li>Google Maps is free until 15,000 requests per day. If this project becomes famous and necessary, I will have to pay for the rest of the usage.</li>
        <li>You do not NEED to donate. Do it if you want.</li>
      </ul>
    </section>
    <section class="erigers-section">
      <div class="self-introduction">
        <h3>My name is Erigers Mamoci</h3>
        <p>
          I am a good spirited entrepreneur and I only did this project because I am grateful to my German teacher Angela & her newly-wed husband Franzjörg invited me to their circle celebrating their union and I want them to have their map wherever they travel into the world and pin everyone they meet in their map of life.
        </p>
      </div>
      <div class="my-avatar">
        <img src="" alt="erigers-avatar-animoji">
      </div>
    </section>
    <section class="photo-gallery">
      <div class="slide">
        <img src="" alt="">
      </div>
      <div class="slide">
        <img src="" alt="">
      </div>
      <div class="slide">
        <img src="" alt="">
      </div>
      <div class="slide">
        <img src="" alt="">
      </div>
    </section>
    <section class="special-thanks-section">
      <h3>special thanks</h3>
      <div class="partner">
        <a href="https://maps.google.com" target="_blank">
          <img src="/google-maps-logo.png" alt="google-maps-logo">
        </a>
      </div>
    </section>
    <footer>
      <p>This project has been brought to you from Angela with love.</p>
    </footer> -->
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
.landing {
  width: 100%;
  min-height: 100vh;
}

// open source section

// erigers section

// photo gallery section

// special thanks section
.special-thanks-section {
  width: 100%;
  background: $color-blue;
  height: auto;
}
.special-thanks-section .partner {
  width: calc(100% / 5);
  overflow: hidden;
}
.special-thanks-section a  {
  width: 100%;
}

.special-thanks-section img {
  width: 100%;
}
// footer
</style>
