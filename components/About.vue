<template>
  <div>
    <section class="section is-normal">
      <h1 class="title has-text-centered">
        About
      </h1>
    </section>
    <div class="content is-medium">
      <quote-card />
      <br />
      In modern Western philosophy, sentience is the ability to experience
      sensations. In different Asian religions, the word 'sentience' has been
      used to translate a variety of concepts. In science fiction, the word
      'sentience' is sometimes used interchangeably with sapience, self
      awareness or consciousness.
      <br /><br />
      In 2020 a team of clinical psychologists, and technology solution
      providers combined their expertise to develop an innovative and proactive
      programme and service to gain insight into employee wellness as well as
      obtain employee feedback around organisational issues and needs. Sentience
      Health, has used a unique combination of psychology and technology to
      create an employee feedback program to serve as an effective platform to
      allow leaders to hear directly from staff and gain insight into
      organisational culture as well as monitor staff wellness.
    </div>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `Services | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
