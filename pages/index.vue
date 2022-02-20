<template>
  <div>
    <navigation-simple />
    <div
      class="mb-20 space-y-20 overflow-hidden sm:mb-32 sm:space-y-32 md:mb-40 md:space-y-40"
    >
      <headers-centered />

      <sections-testimonial-centered />
      <sections-testimonial-grid />
      <sections-feature-simple
        name="Customization"
        title="Extend it, tweak it, change it."
        icon="/media/features/customization.png"
      >
        <template #description>
          <p>
            Tailwind includes an expertly crafted set of defaults
            out-of-the-box, but literally everything can be customized — from
            the color palette to the spacing scale to the box shadows to the
            mouse cursor.
          </p>
          <p>
            Use the tailwind.config.js file to craft your own design system,
            then let Tailwind transform it into your own custom CSS framework.
          </p>
        </template>
      </sections-feature-simple>
      <sections-feature-simple
        name="Dark mode"
        title="Now with Dark Mode."
        icon="/media/features/dark.mode.png"
      >
        <template #description>
          <p class="mt-4 max-w-3xl space-y-6">
            Don’t want to be one of those websites that blinds people when they
            open it on their phone at 2am? Enable dark mode in your
            configuration file then throw
            <code
              class="font-mono text-slate-900 font-medium dark:text-slate-200"
              >dark:</code
            >
            in front of any color utility to apply it when dark mode is active.
            Works for background colors, text colors, border colors, and even
            gradients.
          </p>
        </template>
      </sections-feature-simple>
    </div>
    <footer-simple />
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
