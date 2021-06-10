<template>
  <div id="home-page" class="page-wrapper home-page">
    <site-hero
      title=""
      :subtitle="subtitle"
      :image="featureImage"
      :logo="featureLogo"
      class-name="main"
    >
      <button
        v-if="$siteConfig.newsletter.on"
        class="button is-primary"
        @click="$eventBus.$emit('modal-triggered', 'newsletter-modal')"
      >
        Contact us for more info
      </button>
    </site-hero>
    <main-section theme="one-column">
      <template v-slot:default>
        <about />

        <section class="section is-normal">
          <h1 class="title has-text-centered">
            Our Partners
          </h1>
        </section>

        <partners />

        <section class="section is-normal">
          <h1 class="title has-text-centered">
            Our blog
          </h1>
        </section>
        <posts-grid />
      </template>
    </main-section>
  </div>
</template>

<script>
import { mapState } from 'vuex'
import { setPageData } from '../helper'
import About from '~/components/About'
import Partners from '~/components/Partners'

export default {
  name: 'HomePage',
  head() {
    return {
      title: `Home | ${this.$siteConfig.siteName}`
    }
  },
  components: {
    About,
    Partners
  },
  computed: {
    ...mapState(['title', 'subtitle', 'featureImage', 'featureLogo'])
  },
  fetch({ store, params }) {
    setPageData(store, { slug: 'home' })
  }
}
</script>

<style>
.home-page .under-subtitle {
  border-top: none;
}
</style>
