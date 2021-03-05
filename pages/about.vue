<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Us"
      subtitle="IM Enterprise"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>IM Enterprise</h3>
          <p>
            <strong>
              All types of Toys
            </strong>
          </p>
          <p>
            We are dealing in various type of toys.
          </p>
          <p>
            <strong>
              Name : Mayur Kathiriya
            </strong>
          </p>
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
              Address : 58/ Ganeshdham Society, Opposite Muktidham Estate Nikol
              Gam Road Ahmedabad-382350
            </strong>
          </p>
        </div>
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  }
}
</script>
