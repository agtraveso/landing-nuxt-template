<template>
  <footer class="mt-20 sm:mt-32 md:mt-40 pb-16 text-sm leading-6">
    <div
      class="max-w-7xl mx-auto divide-y divide-slate-200 px-4 sm:px-6 md:px-8 dark:divide-slate-700"
    >
      <div class="flex">
        <div
          class="flex-none w-1/2 space-y-10 sm:space-y-8 lg:flex lg:space-y-0"
        >
          <div
            v-for="category in categories"
            :key="category.name"
            class="lg:flex-none lg:w-1/2"
          >
            <h2 class="font-semibold text-slate-900 dark:text-slate-100">
              {{ category.name }}
            </h2>
            <ul class="mt-3 space-y-2">
              <li v-for="link in category.links" :key="link.name">
                <a
                  class="hover:text-slate-900 dark:hover:text-slate-300"
                  :href="link.href"
                  >{{ link.name }}</a
                >
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="mt-16 pt-10">
        <app-logo />
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterSimple',
  data() {
    return {
      categories: [
        {
          name: 'Getting started',
          links: [
            {
              name: 'Instalation',
              href: '/docs/installation',
            },
            {
              name: 'Browser support',
              href: '/docs/browser-support',
            },
            {
              name: 'Upgrade guide',
              href: '/docs/upgrade-guide',
            },
          ],
        },
        {
          name: 'Core concepts',
          links: [
            {
              name: 'Responsive Design',
              href: '/docs/responsive-design',
            },
            {
              name: 'Dark mode',
              href: '/docs/dark-mode',
            },
          ],
        },
        {
          name: 'Customization',
          links: [
            {
              name: 'Configuration',
              href: '/docs/config',
            },
            {
              name: 'SEO',
              href: '/docs/SEO',
            },
            {
              name: 'Components',
              href: '/docs/components',
            },
            {
              name: 'Deployment',
              href: '/docs/deployment',
            },
            {
              name: 'Theme',
              href: '/docs/theme',
            },
          ],
        },
        {
          name: 'Community',
          links: [
            {
              name: 'Github',
              href: '/github',
            },
          ],
        },
      ],
    }
  },
}
</script>
