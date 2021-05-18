<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Us"
      subtitle=""
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section>
      <template v-slot:default>
        <div class="content">
          <quote-card />
          <br />
          In modern Western philosophy, sentience is the ability to experience
          sensations. In different Asian religions, the word 'sentience' has
          been used to translate a variety of concepts. In science fiction, the
          word 'sentience' is sometimes used interchangeably with sapience, self
          awareness or consciousness.
          <br /><br />In 2020 a team of clinical psychologists, and technology
          solution solution providers combined their expertise to develop an
          innovative and proactive programme and service to gain insight into
          employee wellness as well as obtain employee feedback around
          organisational issues and needs. Sentience Health, has used a unique
          combination of psychology and technology to create an employee
          feedback program to serve as an effective platform to allow leaders to
          hear directly from staff and gain insight into organisational culture
          as well as monitor staff wellness.
        </div>

        <section class="section is-medium">
          <h1 class="title">
            Team
          </h1>
          <h2 class="subtitle">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod eiusmod tempor incididunt ut labore et dolore magna aliqua
          </h2>
        </section>

        <team />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
import Team from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard, Team }
}
</script>
