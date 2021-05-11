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
          In 2020 a team of clinical psychologists, and technology solution
          providers combined their expertise to develop an innovative and
          proactive programme and service to gain insight into employee wellness
          as well as obtain employee feedback around organisational issues and
          needs. Sentience Health, has used a unique combination of psychology
          and technology to create an employee feedback program to serve as an
          effective platform to allow leaders to hear directly from staff and
          gain insight into organisational culture as well as monitor staff
          wellness.
        </div>

        <!-- <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Cool Stuff We Do
              </p>
              <p class="subtitle">
                Sooo Cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Other Cool Things
              </p>
              <p class="subtitle">
                Just as cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                All the cool
              </p>
              <p class="subtitle">
                that is all
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
        </div> -->
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
