<template>
  <footer class="text-gray-600 body-font mb-8">
    <div class="">
      <div
        class="container mx-auto py-4 px-5 flex flex-wrap flex-col sm:flex-row"
      >
        <p class="text-gray-700 text-sm text-center sm:text-left">
          © {{ copyrightYear }} Designed & Built with
          <a href="" class="text-purple-800 font-bold">Nuxt.js</a>,
          <a href="" class="text-purple-800 font-bold">Tailwind.css</a>, and
          many more.
        </p>
      </div>
    </div>
    <div
      class="bg-purple-800 p-2 shadow-lg rounded-full fixed bottom-0 right-0 mr-1 mb-5 cursor-pointer animate__animated animate__jackInTheBox"
      @click="backToTop"
      v-show="scrolledToBottom"
      appear
    >
      <span class="text-gray-800">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6 fill-current text-white"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M5 10l7-7m0 0l7 7m-7-7v18"
          />
        </svg>
      </span>
    </div>
  </footer>
</template>

<script>
export default {
  props: ['scrolledToBottom'],
  data: function () {
    return {
      effects: [
        {
          mainAudio: '/whoosh.mp3',
          duration: 1000,
        },
        {
          mainAudio: '/gun.mp3',
          duration: 900,
        },
        {
          mainAudio: '/fart.mp3',
          duration: 4000,
        },
      ],
    }
  },
  methods: {
    backToTop: function () {
      let { mainAudio, duration } = this.effects[
        Math.floor(Math.random() * this.effects.length)
      ]

      let elevator = new Elevator({
        mainAudio,
        duration,
      })

      elevator.elevate()
    },
  },
  computed: {
    copyrightYear: function () {
      if (new Date().getFullYear() == '2021') {
        return '2021'
      } else return `2021-${new Date().getFullYear()}`
    },
  },
}
</script>

<style></style>
