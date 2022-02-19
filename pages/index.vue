<template>
  <div id="index">
    <Hero />
  </div>
</template>

<script>
import Hero from '~/components/Hero'

export default {
  data: function () {
    return {}
  },
  components: {
    Hero,
  },
  computed: {},
  mounted: function () {
    twemoji.parse(document.body, {
      folder: 'svg',
      ext: '.svg',
    })
  },
}
</script>

<style></style>
