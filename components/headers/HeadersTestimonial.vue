<template>
  <div
    class="max-w-7xl mx-auto px-4 sm:px-6 md:px-8 mt-20 sm:mt-24 lg:mt-32 lg:grid lg:gap-8 lg:grid-cols-12 lg:items-center"
  >
    <div
      class="relative row-start-1 col-start-6 xl:col-start-7 col-span-7 xl:col-span-6"
    >
      <div class="-mx-4 sm:mx-0">
        <div
          class="relative overflow-hidden shadow-xl flex bg-slate-800 h-[31.625rem] max-h-[60vh] sm:max-h-[none] sm:rounded-xl lg:h-[34.6875rem] xl:h-[31.625rem] dark:bg-slate-900/70 dark:backdrop-blur dark:ring-1 dark:ring-inset dark:ring-white/10 !h-auto max-h-[none]"
        >
          <img
            src="~/assets/media/header/security.jpeg"
            alt=""
            class="h-96 w-full"
            loading="lazy"
          />
        </div>
      </div>
    </div>
    <div
      class="relative row-start-1 col-start-1 col-span-5 xl:col-span-6 -mt-10"
    >
      <div
        class="h-[24.25rem] max-w-xl mx-auto lg:max-w-none flex items-center justify-center"
      >
        <div class="w-full flex-none">
          <div class="lg:-mr-18">
            <div
              class="relative z-10 rounded-lg shadow-xl text-slate-900 mx-auto sm:w-[23.4375rem] dark:text-slate-300"
              style="transform-origin: 50% 50% 0px; width: 664px"
            >
              <div
                class="bg-white rounded-lg overflow-hidden ring-1 ring-slate-700 dark:bg-slate-800 dark:highlight-white dark:ring-0 flex p-8"
                style="transform-origin: 50% 50% 0px"
              >
                <div
                  class="absolute z-20 top-1/2 right-0 xl:right-auto xl:left-0 text-black rounded-full -mt-4 -mr-4 xl:mr-0 xl:-ml-4 pointer-events-none"
                  style="opacity: 0; transform-origin: 50% 50% 0px"
                >
                  <svg class="h-8 w-8" viewBox="0 0 100 100">
                    <circle
                      cx="50"
                      cy="50"
                      r="40"
                      stroke="rgba(255, 255, 255, 0.5)"
                      stroke-width="8"
                      fill="rgba(0, 0, 0, 0.5)"
                    ></circle>
                  </svg>
                </div>
                <div
                  class="relative z-10 overflow-hidden flex-none -m-8 mr-8 w-48 h-auto"
                  style="transform-origin: 50% 50% 0px; border-radius: 0%"
                >
                  <img
                    src="~/assets/media/header/ninja_injured.jpeg"
                    alt=""
                    class="absolute max-w-none object-cover bg-slate-100"
                    style="
                      width: 100%;
                      height: 100%;
                      left: 0px;
                      top: 0px;
                      transform-origin: 50% 50% 0px;
                    "
                  />
                </div>
                <div>
                  <div class="text-lg mb-4">
                    "I have fought hundreds of battles against SEO, design
                    fustrations and deployment issues. Nothing is more valuable
                    than having a tool to help you deal with adverse elements.
                    This is the best I found since I born in 1584."
                  </div>
                  <div
                    class="flex flex-col items-start"
                    style="font-weight: 500"
                  >
                    <p
                      class="transition-colors duration-500 text-indigo-500 dark:text-indigo-400"
                      style="transform-origin: 50% 50% 0px"
                    >
                      Miyamoto Musashi
                    </p>
                    <p
                      class="transition-colors duration-500 text-slate-700 dark:text-slate-500"
                      style="transform-origin: 50% 50% 0px"
                    >
                      Swordsman, philosopher, strategist, writer and rōnin
                    </p>
                  </div>
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
  name: 'HeadersTestimonial',
  props: {},
}
</script>
