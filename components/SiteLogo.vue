<template>
  <div class="logo-wrapper">
    <div
      :class="{
        'logo-inner': true,
        blink: blinking
      }"
    >
      <img src="/logo_main.png" />
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
    img {
      display: block;
      height: 82px;
      margin: 5px;
      margin-top: -7px;
      max-height: initial;
    }
  }
}
</style>
