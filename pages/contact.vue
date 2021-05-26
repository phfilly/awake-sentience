<template>
  <div id="contact-page" class="page-wrapper contact-page content-page">
    <site-hero title="Contact Us" image="/uploads/contact-hero.jpg"></site-hero>
    <main-section>
      <template v-slot:default>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Welcome!
              </p>
              <p class="subtitle">
                Where to find us
              </p>
              <p>
                Sentience Health<br />
                45 Tudor Place<br />
                61 Hillcrest Avenue<br />
                Randburg<br />
                South Africa<br />
                <a href="mailto:info@sentiencehealth.com">
                  info@sentiencehealth.com <br /><br />
                </a>
              </p>
              <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3582.583335230353!2d28.016597515445355!3d-26.11251668347872!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x1e957355f68b4b75%3A0x7709a9c7ea22201f!2sTudor%20Park%20Office%20Suites!5e0!3m2!1saf!2sza!4v1622031238097!5m2!1saf!2sza"
                width="600"
                height="1500"
                style="border:0;"
                allowfullscreen=""
                loading="lazy"
              >
              </iframe>
            </article>
          </div>
          <div class="tile is-parent is-8">
            <article class="tile is-child box">
              <contact-form />
            </article>
          </div>
        </div>
      </template>
    </main-section>
  </div>
</template>
<script>
import ContactForm from '~/components/ContactForm'
export default {
  head() {
    return {
      title: `Contact | ${this.$siteConfig.siteName}`
    }
  },
  components: { ContactForm }
}
</script>
