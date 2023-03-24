<template>
  <div>
    <section data-aos="fade-right" data-aos-easing="linear" data-aos-duration="1500"
      class="py-10 mt-15 bg-gray-50 sm:py-16 lg:py-24">
      <div class="px-4 mx-auto max-w-7xl sm:px-6 lg:px-8">
        <div class="text-center">
          <h2 class="text-2xl font-bold leading-tight text-black sm:text-2xl lg:text-5xl">
            3,583 Students are <br />
            already using mentor
          </h2>
        </div>

        <div class="px-5 mt-15 py-8 mt-12 bg-gradient-to-r from-yellow-200 via-pink-200 to-pink-400 lg:mt-20 lg:p-16">
          <div class="grid grid-cols-1 gap-12 lg:gap-16 sm:grid-cols-2">
            <div class="flex items-start">
              <img class="flex-shrink-0 w-16 h-16 text-fuchsia-600" src="~/assets/promotion.png" />

              <div class="ml-5">
                <h3 class="text-lg font-semibold text-white">
                  Grow in your career
                </h3>
                <p class="mt-4 text-base text-gray-600">
                  Build a strong network, Connect with people in your industry
                  or profession.
                </p>
              </div>
            </div>

            <div class="flex items-start">
              <img class="flex-shrink-0 w-16 h-16 text-fuchsia-600" src="~/assets/report.png" />

              <div class="ml-5">
                <h3 class="text-lg font-semibold text-white">
                  Get useful information
                </h3>
                <p class="mt-4 text-base text-gray-600">
                  Gain access to industry-specific resources, networking
                  opportunities, and professional development opportunities.
                </p>
              </div>
            </div>

            <div class="flex items-start">
              <img class="flex-shrink-0 w-16 h-16 text-fuchsia-600" src="~/assets/technology.png" />

              <div class="ml-5">
                <h3 class="text-lg font-semibold text-white">Tech masters</h3>
                <p class="mt-4 text-base text-gray-600">
                  Select tech masters who have not only made significant
                  contributions to the industry but have also inspired and
                  mentored countless others in the field.
                </p>
              </div>
            </div>

            <div class="flex items-start">
              <img class="flex-shrink-0 w-16 h-16 text-fuchsia-600" src="~/assets/backlog.png" />

              <div class="ml-5">
                <h3 class="text-lg font-semibold text-white">
                  Get feedback and advise
                </h3>
                <p class="mt-4 text-base text-gray-600">
                  be specific about your questions and what you hope to learn.
                  Be open to constructive criticism and take the feedback you
                  receive as an opportunity to learn and grow.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
  <promo />
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";
export default {
  mounted() {
    AOS.init({});
  },
};
</script>

<style lang="scss" scoped></style>