<template>
  <div id="skills" class="mb-10">
    <div class="text-gray-900 max-w-screen-xl mx-auto px-4 leading-6">
      <!-- Breadcrumb -->
      <div class="flex text-black">
        <span class="text-md mt-4"><nuxt-link to="/">Home</nuxt-link></span>
        <span class="text-md mt-4 mx-2">></span>
        <h1 class="text-xl font-bold underline mt-4">Skills</h1>
      </div>
      <!-- Breadcrumb -->

      <!-- Technical Skills -->
      <div class="mt-5">
        <h1 class="flex text-2xl font-bold leading-7 text-black">Skills 🚀</h1>
        <div id="programming">
          <h3 class="mt-5 text-xl underline">Programming Language(s)</h3>
          <p class="mt-5">
            Programming language(s) have been the tools used for ages by
            developers for creating software or an application.
          </p>
          <div class="-mx-4 flex flex-wrap">
            <div class="w-full flex flex-col p-4 sm:w-1/2 lg:w-1/3">
              <div
                class="flex flex-col flex-1 px-8 py-10 bg-white rounded-lg border border-gray-300"
              >
                <div class="flex-1">
                  <a href="/" class="text-lg font-bold leading-7 text-black"
                    >JavaScript</a
                  >
                  <p class="mt-2 text-gray-700">
                    <a href="" target="_blank" class="text-purple-800 font-bold"
                      >JavaScript</a
                    >
                    started been a language for the web or the broswer. It makes
                    the web more interactive. Runtime like Node.js makes it
                    possible to bring JavaScript to server-side. Fortunately,
                    JavaScript can now be used for web, server, mobile, and
                    desktop application(s).
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div id="databases">
          <h3 class="mt-5 text-xl underline">Database(s)</h3>
          <p class="mt-5">
            Database is a repository of data. A database can an SQL, NoSQL, or
            Graph database.

            <!-- SQL databases are database . NoSQL database  -->
          </p>
          <div class="-mx-4 flex flex-wrap">
            <div class="w-full flex flex-col p-4 sm:w-1/2 lg:w-1/3">
              <div
                class="flex flex-col flex-1 px-8 py-10 bg-white rounded-lg border border-gray-300"
              >
                <div class="flex-1">
                  <a href="/" class="text-lg font-bold leading-7 text-black"
                    >MySQL</a
                  >
                  <p class="mt-2 text-gray-700">
                    <a href="" target="_blank" class="text-purple-800 font-bold"
                      >MySQL</a
                    >
                    is an SQL database based on rows and columns. MySQL happens
                    to be the best choice when working with financial project
                    because of its ability to perform transactions and roll back
                    when errors occur during the transaction.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  head: {
    title: 'Obafunso Ridwan A. - Skills',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content:
          'Technical and soft skills of Obafunso Ridwan Adebayo. Ridwan is always eager to learn new technology stack to improve his knowledge and career.',
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
