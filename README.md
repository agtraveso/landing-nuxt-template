# Landing NuxJS template

Hi there! This is an extensible Github template with the important stuff preconfigured: `components`, `auto-deploy`, `SEO` and `dark/light theme` that lets you build your landing page without effort.

You can configure it to meet your specific needs.

## First steps

Click `Use this template` button next to clone button, and there you go. If you're curious check the [official docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

#### This is a NuxtJS based project

This means you have the potential of [NuxtJS](https://nuxtjs.org/docs/get-started) on your hands, but we have added for you some content to make you life easier.

To start and seeing the changes you are making start the app in development mode:

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

## components

Take a look the Vue components we added, pick the ones that best fits your needs, tweak and change them!

## assets

Here we added some dummy images and a basic css. Delete and replace with yours.

## Styling & theme colors

We use [Tailwind](https://tailwindcss.com/docs) for styling. Update `tailwind.config.js` with your colors, we mainly use `stale` and `indigo` palettes.

## SEO

Default SEO is configured in `nuxt.config.js`, we've already added some stuff. Check the [official docs](https://nuxtjs.org/docs/features/meta-tags-seo/) for fine tunning.

## Auto deployment

There is a pre-configured GitHub Action for [GitHub Pages](https://pages.github.com/) at [`.github/workflows/cd-gh-pages.yaml`](.github/workflows/cd-gh-pages.yaml).

To make it work go to your settings repository: `Settings` > `Pages` then select the branch `gh-pages` as the source. Every commit in `main` branch will trigger the deployment.

## Troubleshooting

### Deploying to GitHub Pages returns: 404 There isn't a GitHub Pages site here.

Check that your project `name` in `package.json` matches the `router.base` in `nuxt.config.js`

```json nuxt.config.js
  {
  "name": "my-awesome-project",
  "version": "1.0.0"
  ...
  }
```

```js nuxt.config.js
  // https://nuxtjs.org/deployments/github-pages/
  router: {
    base: 'my-awesome-project',
  },
```

## License

Landing NuxtJS template is licensed under the [MIT License](https://github.com/tabler/tabler-icons/blob/master/LICENSE).
