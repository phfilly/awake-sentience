<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Services and Solutions"
      subtitle=""
      image="/uploads/scott-graham-min.jpg"
    ></site-hero>
    <main-section>
      <template v-slot:default>
        <h1 class="title has-text-centered">
          Context
        </h1>
        <div class="content is-medium">
          <br />
          A number of employers underestimate the financial impact that mental
          illness and poor organisational culture has on their bottom-line. Poor
          work culture as well as mental illness in the workplace leads to
          decreased productivity, increased sick-related absenteeism, poor work
          quality, loss of key staff and even compromised workplace safety.
          Despite the significant financial loss to employers, many of these
          crucial issues fly below the radar in the workplace and go unnoticed
          by leaders.<br /><br />
          Untreated mental disorders cost our economy more than R35 billion each
          year, with one in six South Africans suffering from depression or some
          form of mental disorder within their lifetime. Furthermore, bullying,
          conflict, unreasonable hours / demands, overt sexism, and racism are
          all clear signs that the culture of an organisation is potentially
          toxic and likely that productivity and the well-being of people in the
          organisation are affected. During this unprecedented period of change
          and increasing financial constraints of the COVID-19 pandemic, it is
          imperative that staff feel engaged, valued and supported at work, in
          order to protect against mental illness as well as to encourage a
          healthy organisational culture. Therefore, it is more crucial than
          ever for leaders to listen closely and deeply to staff feelings and
          issues, which directly impact their everyday experience within the
          organisation and the organisation itself. Designing and maintaining
          structured, well-organised, and deliberate opportunities for employees
          to share their honest thoughts is an absolute necessity to create an
          atmosphere where a workforce feels valued, connected and engaged, and
          enables leaders to be far more in-tune with all dynamics and possible
          risks within their teams and organisation.
        </div>
        <solution />
      </template>
    </main-section>
  </div>
</template>

<script>
import Solution from '../components/Solution.vue'

export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { Solution }
}
</script>
