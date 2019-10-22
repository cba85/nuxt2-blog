# nuxt-blog

> Nuxt.js project

## Build Setup

``` bash
# install dependencies
$ npm install # Or yarn install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, checkout the [Nuxt.js docs](https://github.com/nuxt/nuxt.js).

## Steps

## 1. Configration

- Install nuxt.js starter template

## 2. Architecture

- Check architecture
- Create about.vue in pages

## 3. HTTP Requests

- https://jsonplaceholder.typicode.com
- Create posts/index.vue
- Change layouts/default.vue

```
npm install axios
```

## 4. Components
- Create components/Post.vue
- Update pages/posts/index.vue

## 5. Sass

Optional:
```
npm install sass-loader node-sass --save
```

- Add scss in Post.vue
- Create app.scss in assets
- Create layout/_container.scss in assets
- Add css in nuxt.config.js

## 6. Route parameters

- Create pages/_id.vue

## 7. Vendor dependencies

- Add vendor in build in nuxt.config.js

## 8. Link

- Add nuxt-link in components/Post.vue

## 9. Page title and meta

- Update head in nuxt.config.js
- add head in index.vue
- add head in _id.vue

## 10. Layouts

- add bootstap in nuxt.config.js
- create layouts/posts.vue
- add layout in posts/index.vue

## 11. Mixins

- add posts.length in pages/posts/index.vue
- install https://www.npmjs.com/package/pluralize
- add pluralize in pages/posts/index.vue
- remove pluralize from pages/posts/index.vue
- create plugins/mins/pluralize.js
- add plugin in nuxt.config.js

## 12. Custom errors page

- create layouts/error.vue
- add try/catch in pages/posts/_id.vue

## 13. Plugin

- install https://www.npmjs.com/package/vue-scrollto
- create plugins/scrooTo.js
- add plugin in nuxt.config.js

## 14. Client only plugins

- Install https://github.com/sagalbot/vue-select
- create plugins/vueSelect.js
- add plugin in nuxt.config.js
- add selection in pages/posts/index.vue