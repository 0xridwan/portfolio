<template>
  <div id="biography" class="mb-10">
    <div class="text-gray-900 max-w-screen-xl mx-auto px-4 leading-7">
      <!-- Breadcrumb -->
      <div class="flex text-black">
        <span class="text-md mt-4"><nuxt-link to="/">Home</nuxt-link></span>
        <span class="text-md mt-4 mx-2">></span>
        <h1 class="text-xl font-bold underline mt-4">Biography</h1>
      </div>
      <!-- Breadcrumb -->

      <div class="mt-5">
        <div id="background">
          <h1 class="flex text-2xl font-bold leading-7 text-black">
            Background 📌
          </h1>
          <p class="mt-5">
            <b>Obafunso Ridwan Adebayo</b> (born 19th December) is a Nigerian
            Software Engineer, Researcher, and Entreprenuer. He is passionate
            about technology. His passion drives him to start learning
            programming at a very tender age when he was still in high school.
          </p>
        </div>

        <div class="mt-10" id="background">
          <h1 class="flex text-2xl font-bold leading-7 text-black">
            Education 🧑‍🎓
          </h1>
          <p class="mt-5">
            Ridwan bagged National Diploma in Computer Science at Federal
            Polytechnic, Ilaro which is located in Ogun, Nigeria.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  head: {
    title: 'Obafunso Ridwan A. - Biography',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content:
          'Biography about Obafunso Ridwan Adebayo. Ridwan is always eager to learn new technology stack to improve his knowledge and career.',
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
