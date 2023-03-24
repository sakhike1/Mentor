<template>
  <div class="isolate bg-white">
    <Nav />
    <div class="absolute inset-x-0 top-[-10rem] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[-20rem]">
      <svg
        class="relative left-[calc(50%-11rem)] -z-10 h-[21.1875rem] max-w-none -translate-x-1/2 rotate-[30deg] sm:left-[calc(50%-30rem)] sm:h-[42.375rem]"
        viewBox="0 0 1155 678">
        <path fill="url(#45de2b6b-92d5-4d68-a6a0-9b9b2abad533)" fill-opacity=".3"
          d="M317.219 518.975L203.852 678 0 438.341l317.219 80.634 204.172-286.402c1.307 132.337 45.083 346.658 209.733 145.248C936.936 126.058 882.053-94.234 1031.02 41.331c119.18 108.451 130.68 295.337 121.53 375.223L855 299l21.173 362.054-558.954-142.079z" />
        <defs>
          <linearGradient id="45de2b6b-92d5-4d68-a6a0-9b9b2abad533" x1="1155.49" x2="-78.208" y1=".177" y2="474.645"
            gradientUnits="userSpaceOnUse">
            <stop stop-color="#9089FC" />
            <stop offset="1" stop-color="#FF80B5" />
          </linearGradient>
        </defs>
      </svg>
    </div>

    <div data-aos="fade-up" data-aos-duration="3000" class="px-8 pt-12 mx-auto max-w-7xl sm:px-12 lg:px-8">
      <div class="grid items-center grid-cols-1 gap-12 lg:grid-cols-2">
        <div>
          <p class="text-base font-semibold tracking-wider text-blue-600 uppercase">
            A social media for learners
          </p>
          <h1 class="mt-4 text-4xl font-bold text-black lg:mt-8 sm:text-6xl xl:text-8xl">
            Connect & learn from the experts
          </h1>
          <p class="mt-4 text-base text-black lg:mt-8 sm:text-xl">
            Grow your career fast with the right mentor.
          </p>
          <a href="#_"
            class="relative mt-2 inline-flex transition-all duration-500 ease-out hover:bg-green-500 group-hover:w-56 group-hover:h-56 items-center justify-center px-10 py-4 overflow-hidden font-mono font-medium tracking-tighter text-white bg-gray-800 rounded-lg group">
            <span class="relative">Learn More</span>
          </a>

          <p class="mt-5 text-gray-600">
            Already joined us?
            <nuxt-link class="text-black transition-all duration-200 hover:underline" to="Signin"> Log
              in</nuxt-link>
          </p>
        </div>

        <div>
          <img class="w-full" src="https://cdn.rareblocks.xyz/collection/celebration/images/hero/1/hero-img.png" alt="" />
        </div>
      </div>
    </div>
    <Mentor />
  </div>
  <Footer />
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";
import carousel from "./carousel.vue";
export default {
  components: { carousel },
  mounted() {
    AOS.init({});
  },
};
</script>

<style  scoped></style>