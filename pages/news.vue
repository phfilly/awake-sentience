<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="In The News"
      subtitle=""
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section>
      <template v-slot:default>
        <posts-grid />
      </template>
    </main-section>
    <news-letter-form-modal />
  </div>
</template>
<script>
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
