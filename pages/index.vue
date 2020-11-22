<template>
  <HomePage prefix="homePage" :content="md" />
</template>

<script>
import HomePage from '~/components/HomePage.vue'
export default {
  name: 'Index',
  components: {
    HomePage,
  },
  async asyncData({ $content }) {
    const md = await $content('indexPage/index').fetch()
    return {
      md,
    }
  },
  head() {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' },
      ],
    }
  },
}
</script>

<style>
/* .container {
		  margin: 0 auto;
		  min-height: 100vh;
		  display: flex;
		  justify-content: center;
		  align-items: center;
		  text-align: center;
		} */
</style>
