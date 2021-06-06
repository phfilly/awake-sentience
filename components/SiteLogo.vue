<template>
  <div class="logo-wrapper">
    <div
      :class="{
        'logo-inner': true,
        blink: blinking
      }"
    >
      <!-- <img src="/logo_main.png" /> -->
    </div>
  </div>
</template>
<script>
export default {
  name: 'SiteLogo',
  data() {
    return {
      frames: 5,
      currentFrame: 1,
      blinking: false
    }
  }
}
</script>
<style lang="scss">
@keyframes logoBlink {
  100% {
    transform: translateY(-360px);
  }
}
.logo-wrapper {
  position: relative;
  height: 66px;
  overflow: hidden;
  margin-top: -5px;
  width: 200px;
  .logo-inner {
    position: absolute;
    height: 500px;
    img {
      display: block;
      height: 70px;
      margin: 5px;
      max-height: initial;
    }
    &.blink {
      animation: logoBlink 0.2s steps(8, end) alternate;
    }
  }
}
</style>
