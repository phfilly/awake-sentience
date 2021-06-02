<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Partners"
      subtitle=""
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section>
      <template v-slot:default>
        <partners />
      </template>
    </main-section>
  </div>
</template>
<script>
// import QuoteCard from '~/components/cards/QuoteCard'
// import TeamCard from '~/components/cards/QuoteCard'
import Partners from '../components/Partners.vue'

export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { Partners }
}
</script>
