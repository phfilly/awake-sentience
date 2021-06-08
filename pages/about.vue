<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Meet the team"
      subtitle=""
      image="/uploads/leon.jpg"
    ></site-hero>
    <main-section>
      <template v-slot:default>
        <team />
      </template>
    </main-section>
  </div>
</template>
<script>
import Team from '~/components/Team'

export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { Team }
}
</script>
