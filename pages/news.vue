<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="In The News"
      subtitle=""
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section>
      <template v-slot:default>
        <news-letter-form-modal />
      </template>
    </main-section>
  </div>
</template>
<script>
// import QuoteCard from '~/components/cards/QuoteCard'
// import TeamCard from '~/components/cards/QuoteCard'
import NewsLetterFormModal from '~/components/NewsLetterFormModal'

export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { NewsLetterFormModal }
}
</script>
