<template>
  <div>
    <Hero />
    <Champion />
    <Questions />
  </div>
</template>

<script>
import Hero from '~/components/startadojo/Hero';
import Champion from '~/components/startadojo/Champion';
import Questions from '~/components/startadojo/Questions';
export default {
  head () {
    return {
      title: this.$t('Start a CoderDojo club in your local area'),
      meta: [
        { hid: 'description', name: 'description', property: 'description', content: this.$t('Starting a Dojo is a fun and incredibly rewarding experience. The most important attribute you should have is that you can bring people together for a shared goal. Our registration process will guide you every step of the way making sure you have the most useful resources to hand.') },
        { hid: 'og:description', name: 'og:description', property: 'og:description', content: this.$t('Starting a Dojo is a fun and incredibly rewarding experience. The most important attribute you should have is that you can bring people together for a shared goal. Our registration process will guide you every step of the way making sure you have the most useful resources to hand.') },
        { hid: 'og:title', name: 'og:title', property: 'og:title', content: this.$t('Start a CoderDojo club in your local area') },
        { hid: 'og:site-name', name: 'og:site-name', property: 'og:site-name', content: 'CoderDojo' },
        { hid: 'og:url', name: 'og:url', property: 'og:url', content: 'https://coderdojo.com/start-a-dojo/' },
        { hid: 'og:type', name: 'og:type', property: 'og:type', content: 'website' },
        { hid: 'og:image', name: 'og:image', property: 'og:image', content: '~/static/images/startadojo/meta-header.png' },
        { hid: 'twitter:title', name: 'twitter:title', property: 'twitter:title', content: this.$t('Start a CoderDojo club in your local area') },
        { hid: 'twitter:url', name: 'twitter:url', property: 'twitter:url', content: 'https://coderdojo.com/start-a-dojo/' },
        { hid: 'twitter:image', name: 'twitter:image', property: 'twitter:image', content: '~/static/images/startadojo/meta-header.png' },
        { hid: 'twitter:description', name: 'twitter:description', property: 'twitter:description', content: this.$t('Starting a Dojo is a fun and incredibly rewarding experience. The most important attribute you should have is that you can bring people together for a shared goal. Our registration process will guide you every step of the way making sure you have the most useful resources to hand.') },
        { hid: 'twitter:card', name: 'twitter:card', property: 'twitter:card', content: 'summary_large_image' }
      ]
    }
  },
  components: {
    Hero,
    Champion,
    Questions,
  },
};
</script>

<style lang="scss" scoped>
</style>
