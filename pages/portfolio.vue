<template>
  <div id="Portfolio" class="mb-10">
    <div class="text-gray-900 max-w-screen-xl mx-auto px-4 leading-6">
      <!-- Breadcrumb -->
      <div class="flex text-black">
        <span class="text-md mt-4"><nuxt-link to="/">Home</nuxt-link></span>
        <span class="text-md mt-4 mx-2">></span>
        <h1 class="text-xl font-bold underline mt-4">Portfolio</h1>
      </div>
      <!-- Breadcrumb -->

      <!-- Technical Portfolio -->
      <div class="mt-5">
        <h1 class="flex text-2xl font-bold leading-7 text-black">
          Portfolio 🚀
        </h1>

        <div id="programming">
          <h3 class="mt-5 text-xl underline">Web Application</h3>
          <div class="-mx-4 flex flex-wrap">
            <p class="p-4 font-bold">None at the moment!!!</p>
          </div>
        </div>

        <div id="programming">
          <h3 class="mt-5 text-xl underline">Mobile Application</h3>
          <div class="-mx-4 flex flex-wrap">
            <p class="p-4 font-bold">None at the moment!!!</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  head: {
    title: 'Obafunso Ridwan A. - Portfolio',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content:
          'Technical and soft Portfolio of Obafunso Ridwan Adebayo. Ridwan is always eager to learn new technology stack to improve his knowledge and career.',
      },
    ],
  },
  mounted: function () {
    twemoji.parse(document.body, {
      folder: 'svg',
      ext: '.svg',
    })
  },
}
</script>

<style></style>
