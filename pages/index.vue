<script>
import bootstrap from '../components/bootstrap.vue'
import footerVue from '../components/footer.vue'
export default {
  components: {
    bootstrap,
    footerVue
  },
  head: {
    title: 'Home page',
    meta: [
      {
        hid: 'description',
        name: 'description',
        content: 'Home page description'
      }
    ]
  }
}
</script>
<template>
  <main>
    <div>
      <bootstrap />
    </div>
    <div class="max-w-screen-xl mx-auto text-center mt-8 lg:mt-20 xl:mt-32 mb-8 lg:mb-20 xl:mb-32">
      <h2 class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl text-gray-700 font-medium">Buy our awesome product now</h2>
      <p class="text-xl  text-gray-600 mt-4 max-w-3xl mx-auto">World among the stalks, and grow familiar with the countless indescribable forms of the insects and flies, then I feel the presence of the Almighty, who formed us in his own image, and the breath</p>
      <a href="/" class="inline-block  bg-gray-600 font-semibold rounded-lg py-4 px-5 lg:px-8 text-white mt-6">Order now</a>
    </div>

    <div class="max-w-screen-xl mx-auto px-6 lg:px-8 xl:px-4 grid grid-cols-2 sm:grid-cols-3 space-y-5 sm:space-y-3 xl:grid-cols-6 col-gap-6 mt-8 lg:mt-10 mb-12 lg:mb-20">
      <img class="h-12 p-1 self-end justify-self-center opacity-90" src="/images/boxify-logo.svg" alt="logo placeholder">
      <img class="h-10 p-1 self-end justify-self-center opacity-90" src="/images/edge-logo.svg" alt="logo placeholder">
      <img class="h-10 p-1 self-end justify-self-center opacity-90" src="/images/sbalbew-logo.svg" alt="logo placeholder">
      <img class="h-10 p-1 self-end justify-self-center opacity-90" src="/images/drops-logo.svg" alt="logo placeholder">
      <img class="h-12 p-1 self-end justify-self-center opacity-90" src="/images/pathway-logo.svg" alt="logo placeholder">
      <img class="h-12 p-1 self-end justify-self-center opacity-90" src="/images/feedback-logo.svg" alt="logo placeholder">
    </div>

  </div>

    <div class="bg-gray-50 text-gray-600 px-6 lg:px-8 pt-12 pb-20">
      <div class="max-w-screen-xl mx-auto">
        <h2 class="text-2xl sm:text-3xl md:text-4xl text-gray-700 font-medium text-center">Amazing Features</h2>
        <p class="text-xl lg:text-2xl text-gray-600 mt-2 text-center">We are mmitted to a unique, cutting-edge approach to that</p>
      </div>
      <div class="md:grid md:grid-cols-2 md:gap-12 max-w-screen-xl mx-auto mt-12 lg:mt-20 space-y-12 md:space-y-0">
        <div class="text-left flex space-x-6">
          <div class="bg-gray-200 rounded-full w-16 h-16 flex items-center justify-center ">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="w-8">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 10h18M7 15h1m4 0h1m-7 4h12a3 3 0 003-3V8a3 3 0 00-3-3H6a3 3 0 00-3 3v8a3 3 0 003 3z" />
            </svg>
          </div>
          <div class="flex-1">
            <h3 class="font-semibold text-lg mb-2">A collection of textile samples</h3>
            <p>One morning, when Gregor Samsa woke from troubled dreams, he found himself It showed transformed in his bed into a horrible vermin.</p>
          </div>
        </div>
        <div class="text-left flex space-x-6">
          <div class="bg-gray-200 rounded-full w-16 h-16 flex items-center justify-center ">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="w-8">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" />
            </svg>
          </div>
          <div class="flex-1">
            <h3 class="font-semibold text-lg mb-2">How about if I sleep a little bit</h3>
            <p>Doing business like this takes much more effort than doing your own business at home, and on top of that there's the curse of travelling.</p>
          </div>
        </div>
        <div class="text-left flex space-x-6">
          <div class="bg-gray-200 rounded-full w-16 h-16 flex items-center justify-center ">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="w-8">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 7v10c0 2.21 3.582 4 8 4s8-1.79 8-4V7M4 7c0 2.21 3.582 4 8 4s8-1.79 8-4M4 7c0-2.21 3.582-4 8-4s8 1.79 8 4m0 5c0 2.21-3.582 4-8 4s-8-1.79-8-4" />
            </svg>
          </div>
          <div class="flex-1">
            <h3 class="font-semibold text-lg mb-2">He felt a slight itch up on his bell</h3>
            <p>He must have tried it a hundred times, shut his eyes so that he wouldn't have to look at the floundering legs, and only stopped when.</p>
          </div>
        </div>
        <div class="text-left flex space-x-6">
          <div class="bg-gray-200 rounded-full w-16 h-16 flex items-center justify-center ">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="w-8">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M9 19l3 3m0 0l3-3m-3 3V10" />
            </svg>
          </div>
          <div class="flex-1">
            <h3 class="font-semibold text-lg mb-2">But who knows, maybe that would do it</h3>
            <p>You've got to get enough sleep. Other travelling salesmen live a life of luxury. For instance, whenever I go back to the guest.</p>
          </div>
        </div>
      </div>
    </div>

    <div class="bg-gray-50 text-gray-600 px-6 lg:px-8 py-12">
      <div class="max-w-screen-xl mx-auto grid md:grid-cols-2 lg:grid-cols-3 gap-6 lg:gap-x-8">
        <div class="bg-gray-200 px-6 pt-20 lg:pt-32 xl:pt-48 pb-6 rounded">
          <h3 class="font-semibold text-lg mb-2">Collection of textile</h3>
          <p>One morning, when Gregor Samsa woke from troubled dreams, he found It showed transformed.</p>
        </div>

        <div class="bg-gray-200 px-6 pt-20 lg:pt-32 xl:pt-48 pb-6 rounded">
          <h3 class="font-semibold text-lg mb-2">How about sleep a little bit</h3>
          <p>Doing business like this takes much more effort than doing your own business at home, on top.</p>
        </div>

        <div class="bg-gray-200 px-6 pt-20 lg:pt-32 xl:pt-48 pb-6 rounded">
          <h3 class="font-semibold text-lg mb-2">But who knows, would do it</h3>
          <p>You've got to get enough sleep. Other travelling salesmen live a life of luxury. For instance.</p>
        </div>
      </div>
    </div>

    <div>
      <footer-vue />
    </div>
  </main>
</template>
