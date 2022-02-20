<template>
  <section
    tabindex="-1"
    class="relative max-w-7xl mx-auto px-4 focus:outline-none sm:px-3 md:px-5"
  >
    <h2 class="sr-only">Testimonials</h2>
    <div
      class="grid grid-cols-1 gap-6 lg:gap-8 sm:grid-cols-2 lg:grid-cols-3 max-h-[33rem] overflow-hidden"
    >
      <ul class="space-y-8">
        <li
          v-for="(testimonial, index) in testimonials.default"
          :key="testimonial.name"
          class="text-sm leading-6"
        >
          <testimonials-card
            :name="testimonial.name"
            :position="testimonial.position"
            :quote="testimonial.quote"
            :avatar="require(`~/assets/media/avatar.0${index}.png`)"
          />
        </li>
      </ul>
      <ul class="space-y-8 hidden sm:block">
        <li
          v-for="(testimonial, index) in testimonials.sm"
          :key="testimonial.name"
          class="text-sm leading-6"
        >
          <testimonials-card
            :name="testimonial.name"
            :position="testimonial.position"
            :quote="testimonial.quote"
            :avatar="
              require(`~/assets/media/avatar.0${
                index + testimonials.default.length
              }.png`)
            "
          />
        </li>
      </ul>
      <ul class="space-y-8 hidden lg:block">
        <li
          v-for="(testimonial, index) in testimonials.lg"
          :key="testimonial.name"
          class="text-sm leading-6"
        >
          <testimonials-card
            :name="testimonial.name"
            :position="testimonial.position"
            :quote="testimonial.quote"
            :avatar="
              require(`~/assets/media/avatar.0${
                index + testimonials.default.length * 2
              }.png`)
            "
          />
        </li>
      </ul>
    </div>
    <div
      class="inset-x-0 bottom-0 flex justify-center bg-gradient-to-t from-white pt-32 pb-8 pointer-events-none dark:from-slate-900 absolute"
    >
      <button
        type="button"
        class="relative bg-slate-900 hover:bg-slate-700 focus:outline-none focus:ring-2 focus:ring-slate-400 focus:ring-offset-2 text-sm text-white font-semibold h-12 px-6 rounded-lg flex items-center dark:bg-slate-700 dark:hover:bg-slate-600 pointer-events-auto"
      >
        Show more...
      </button>
    </div>
  </section>
</template>

<script>
export default {
  name: 'TestimonialGrid',
  data() {
    return {
      testimonials: {
        default: [
          {
            name: 'Rick',
            position: 'Surveyor',
            quote: 'I feel like an idiot for not using this stuff until now.',
          },
          {
            name: 'Donald Rodriguez',
            position: 'Fisherman',
            quote:
              'This great stuff is the most valuable business resource we have EVER purchased. Buy this now. Without this great stuff, we would have gone bankrupt by now.',
          },
        ],
        sm: [
          {
            name: 'Morty',
            position: 'Scaffolder',
            quote:
              "Thanks guys, keep up the good work! I'm good to go. This stuff is the real deal!",
          },
          {
            name: 'Carlie W',
            position: 'Pest controller',
            quote: "Fantastic, I'm totally blown away by this stuff.",
          },
        ],
        lg: [
          {
            name: 'Marie Curie',
            position: 'Toilet attendant',
            quote:
              'This is unbelievable. After using this stuff my business skyrocketed!',
          },
          {
            name: 'Dianna Q.',
            position: 'Carpet fitter',
            quote:
              'This stuff is awesome! I would like to personally thank you for your outstanding product.',
          },
        ],
      },
    }
  },
}
</script>
