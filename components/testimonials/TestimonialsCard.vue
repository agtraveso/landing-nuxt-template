<template>
  <figure
    class="relative flex flex-col-reverse bg-slate-50 rounded-lg p-6 dark:bg-slate-800 dark:highlight-white/5"
  >
    <blockquote class="mt-6 text-slate-700 dark:text-slate-300">
      <p>{{ quote }}</p>
    </blockquote>
    <figcaption class="flex items-center space-x-4">
      <img
        :src="avatar"
        alt=""
        class="flex-none w-14 h-14 rounded-full object-cover"
        loading="lazy"
      />
      <div class="flex-auto">
        <div class="text-base text-slate-900 font-semibold dark:text-slate-300">
          <span class="absolute inset-0"></span>{{ name }}
        </div>
        <div class="mt-0.5">{{ position }}</div>
      </div>
    </figcaption>
  </figure>
</template>

<script>
export default {
  name: 'TestimonialsCard',
  props: {
    name: {
      type: String,
      required: true,
    },
    position: {
      type: String,
      required: true,
    },
    quote: {
      type: String,
      required: true,
    },
    avatar: {
      type: String,
      required: true,
    },
  },
}
</script>
