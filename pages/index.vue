<template>
  <div class="home-container">
    <div class="u-full-width">
      <h1 class="site-title">
          AJF<span class="txt-color"> static </span>Portfolio
      </h1>
       <a class="no-highlighter" href="https://github.com/AJ-Ferguson123/portfolio3" target="_blank">
       <div class="glitch" data-text="Portfolio">Portfolio</div>
        <button class=" repo button-primary">
          See the Repo's
        </button>
      </a>

    </div>
    <script async src="https://identity.netlify.com/v1/netlify-identity-widget.js"></script>
  </div>
</template>

<script>
export default {
  // Define SEO Variables / Site Title, etc.
  head() {
    return {
      title: this.siteName || 'Home Page',
      meta: [
      { hid: 'description',
      name: 'description',
      content: 'A website created with Nuxt Static Skeleton' }
      ]
    };
  },
  async asyncData({ env }) {
    const siteName = env.SITE_NAME
    return {
      siteName
    }
  }
}
</script>

