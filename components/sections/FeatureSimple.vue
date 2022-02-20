<template>
  <section :id="name">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 md:px-8">
      <div
        class="feature-icon w-16 h-16 p-1 rounded-full ring-1 ring-slate-100 overflow-hidden dark:bg-slate-500"
      >
        <img
          :src="icon"
          alt=""
          class="flex-none w-14 h-14 rounded-full object-cover"
          loading="lazy"
        />
      </div>
      <h2 class="mt-8 font-semibold text-pink-500 dark:text-pink-400">
        {{ name }}
      </h2>
      <p
        class="mt-4 text-3xl sm:text-4xl text-slate-900 font-extrabold tracking-tight dark:text-slate-50"
      >
        {{ title }}
      </p>
      <div class="mt-4 max-w-3xl space-y-6">
        <slot name="description" />
      </div>
      <a
        class="group inline-flex items-center h-9 rounded-full text-sm font-semibold whitespace-nowrap px-3 focus:outline-none focus:ring-2 bg-pink-50 text-pink-600 hover:bg-pink-100 hover:text-pink-700 focus:ring-pink-600 dark:bg-slate-700 dark:text-slate-100 dark:hover:bg-slate-600 dark:hover:text-white dark:focus:ring-slate-500 mt-8"
        href="/docs/configuration"
        >Learn more<span class="sr-only">, configuration</span
        ><svg
          class="overflow-visible ml-3 text-pink-300 group-hover:text-pink-400 dark:text-slate-500 dark:group-hover:text-slate-400"
          width="3"
          height="6"
          viewBox="0 0 3 6"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <path d="M0 0L3 3L0 6"></path></svg
      ></a>
      <div class="mt-10">
        <div class="flex overflow-auto -mx-4 sm:mx-0">
          <ul
            class="flex-none inline-grid gap-x-2 px-4 sm:px-0 xl:gap-x-6"
            style="grid-template-columns: repeat(4, minmax(6rem, 1fr))"
          >
            <li>
              <button
                type="button"
                class="group text-sm font-semibold w-full flex flex-col items-center text-pink-500 dark:text-pink-400"
              >
                <svg
                  width="48"
                  height="48"
                  fill="none"
                  aria-hidden="true"
                  class="mb-6 text-pink-500 dark:text-pink-400"
                >
                  <path
                    d="M5 11a4 4 0 0 1 4-4h30a4 4 0 0 1 4 4v26a4 4 0 0 1-4 4H9a4 4 0 0 1-4-4V11Z"
                    fill="currentColor"
                    fill-opacity=".1"
                    stroke="currentColor"
                    stroke-width="2"
                  ></path>
                  <path
                    d="M15 7v34"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                  ></path></svg
                >Simple
              </button>
            </li>
            <li>
              <button
                type="button"
                class="group text-sm font-semibold w-full flex flex-col items-center"
              >
                <svg
                  width="48"
                  height="48"
                  fill="none"
                  aria-hidden="true"
                  class="mb-6 text-slate-300 group-hover:text-slate-400 dark:text-slate-600 dark:group-hover:text-slate-500"
                >
                  <path
                    d="M5 8h36v32H5V8Z"
                    fill="currentColor"
                    fill-opacity="0"
                  ></path>
                  <path
                    d="M42 29V11a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v26a4 4 0 0 0 4 4h19"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                  ></path>
                  <path
                    d="M33.662 41.736a1 1 0 0 1-1.1-1.322l3.08-8.68a1 1 0 0 1 1.736-.274l5.6 7.299a1 1 0 0 1-.637 1.596l-8.679 1.38Z"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  ></path>
                  <path
                    d="M14 7v34"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                  ></path>
                  <path
                    d="M22.8 19.949a2 2 0 0 1 2.4-1.5l5.851 1.352a2 2 0 0 1 1.5 2.399l-1.352 5.851a2 2 0 0 1-2.399 1.5l-5.851-1.352a2 2 0 0 1-1.5-2.399l1.352-5.851Z"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  ></path></svg
                >Playful
              </button>
            </li>
            <li>
              <button
                type="button"
                class="group text-sm font-semibold w-full flex flex-col items-center"
              >
                <svg
                  width="48"
                  height="48"
                  fill="none"
                  aria-hidden="true"
                  class="mb-6 text-slate-300 group-hover:text-slate-400 dark:text-slate-600 dark:group-hover:text-slate-500"
                >
                  <path
                    d="M6 8h32a4 4 0 0 1 4 4v28H6V8Z"
                    fill="currentColor"
                    fill-opacity="0"
                  ></path>
                  <path
                    d="M43 21v16a4 4 0 0 1-4 4H9a4 4 0 0 1-4-4V11a4 4 0 0 1 4-4h20M15 7v34"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                  ></path>
                  <path
                    d="M37 7c0 1.101 0 6-6 6 1.101 0 6 0 6 6 0-6 4.899-6 6-6-6 0-6-4.899-6-6ZM31 21c0 .734 0 4-4 4 .734 0 4 0 4 4 0-4 3.266-4 4-4-4 0-4-3.266-4-4Z"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  ></path></svg
                >Elegant
              </button>
            </li>
            <li>
              <button
                type="button"
                class="group text-sm font-semibold w-full flex flex-col items-center"
              >
                <svg
                  width="48"
                  height="48"
                  fill="none"
                  aria-hidden="true"
                  class="mb-6 text-slate-300 group-hover:text-slate-400 dark:text-slate-600 dark:group-hover:text-slate-500"
                >
                  <path
                    d="M9 41h30a4 4 0 0 0 4-4V11a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v26a4 4 0 0 0 4 4Z"
                    fill="currentColor"
                    fill-opacity="0"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                  ></path>
                  <path
                    d="M15 7v34M17 13h-2M43 13h-6"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                  ></path>
                  <path
                    d="M21 29V15a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2h-8a2 2 0 0 1-2-2Z"
                    fill="none"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                  ></path>
                  <path
                    d="M25 31v2a2 2 0 0 0 2 2h8a2 2 0 0 0 2-2V19a2 2 0 0 0-2-2h-2"
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                  ></path></svg
                >Brutalist
              </button>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'FeatureSimple',
  props: {
    name: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
    icon: {
      type: String,
      required: true,
    },
  },
}
</script>

<style lang="postcss" scoped>
.dark .feature-icon {
  box-shadow: inset 0 1px 0 0 rgb(255 255 255 / 30%);
}
</style>
