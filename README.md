# The Digital Systems Field Guide: Basics

## 🚀 Project Structure

Inside the project, powered by Starlight, you'll see the following folders and files:

```
.
├── public/
├── src/
│   ├── assets/
│   ├── content/
│   │   ├── docs/
│   │   └── config.ts
│   └── env.d.ts
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

Starlight looks for `.md` or `.mdx` files in the `src/content/docs/` directory. Each file is exposed as a route based on its file name.

Images can be added to `src/assets/` and embedded in Markdown with a relative link.

Static assets, like favicons, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:3000`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |


## Custom Components

### Image Swiper

To use the image swiper, import the component and pass in an array of image paths. The component will automatically generate a swiper with the images.

```jsx
// import the component (may need to adjust the level of the import)
import MySwiper from '../../../../../components/react/myswiper.jsx'

// pass in an array of image paths
<MySwiper client:only images={[
  "/test.jpeg",
  "/test.jpeg",
  "/test.jpeg",
]}></MySwiper>
```

Note: files in the public directory are served at the root path.
Instead of /public/test.jpeg, use /test.jpeg.

## 👀 Want to learn more?

Check out [Starlight’s docs](https://starlight.astro.build/), read [the Astro documentation](https://docs.astro.build), or jump into the [Astro Discord server](https://astro.build/chat).

Programmers Field Guide is licensed under [CC BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/?ref=chooser-v1)


