<template>
  <div id="contact-page" class="page-wrapper contact-page content-page">
    <site-hero
      title="Contact Us"
      subtitle="Example Contact Page"
      image="/uploads/contact-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="tile is-ancestor">
          <div class="tile is-parent is-10">
            <article class="tile is-child box">
              <p class="title">
                Hello We are IM Enterprise!
              </p>
              <p class="subtitle">
                What can I do for you?
              </p>

              <br />
              <div class="content">
                <p>
                  <strong>
                    Mobile : +91 9624597809
                  </strong>
                </p>
                <p>
                  <strong>
                    Email : imenterprise.mayur@gmail.com
                  </strong>
                </p>
                <p>
                  <strong>
                    Address : 58/ Ganeshdham Society, Opposite Muktidham Estate
                    Nikol Gam Road Ahmedabad-382350
                  </strong>
                </p>
              </div>
            </article>
          </div>
        </div>
      </template>
      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <!-- Latest Posts -->
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `Contact | ${this.$siteConfig.siteName}`
    }
  }
}
</script>
