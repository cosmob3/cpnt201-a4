# CPNT-201 / Nuxt Framework Setup a-4 / Bryan Velasco

## Repo

[Github Repo](https://github.com/cosmob3/cpnt201-a4)

## Attributions

[npm run serve unsupported code: 'ERR OSSL EVP UNSUPPORTED'](https://www.youtube.com/watch?v=ypHphKXRKAg&t=355s) by FV Tutorial 

- Video is in Portuguese but I can understand the language and it really helped. I was having issues just using `npm run dev` because I was running node.js version `17.6.0`. Had to downgrade to `16.14.0 LTS` and it worked just fine.  

## npm package: 

- [svg-module](https://github.com/nuxt-community/svg-module)

- It allows one to upload svg file. The reason you would want to use svg images specially is because they maintain their resolution no matter how big or how small you make them. 


## Commits 
   1. inital commit

   2. npm project initialized

   3. added 'tailwind.config.js' file

   4. added assets/css/tailwind.css

   5. fully installed and set up tailwind

   6. Installed nuxt/image

   7. installed storyblok

   8. installed nuxtjs/svg

   9. keep getting an error associated with ./node_modules/@storyblok/nuxt/dist/storyblok-nuxt.mjs
   
   
  ![VScode Error](https://user-images.githubusercontent.com/97326786/156517309-1c570a8d-4173-4bf8-9ab6-3f2154c0b970.png)

   10. ran a few audits... more det. in readme
   ![Error2](https://user-images.githubusercontent.com/97326786/156517440-dcb4abeb-10cb-479f-bfc0-0f666ca7aaa1.png)


    - After a couple of audits I started getting a different error message referring to the `svg-module`. Wasn't too sure what to do. I was looking at the Error seeing if I could fix it.
    - I did a `git status` and that showed me that there had been some changes in my `package.json` & `package-lock.json`.
    - When I went and checked them and found svg, it looked like this `@nuxtjs/svg": "^0.0.0"`and if it's all zeros then its not pulling anything. 
    - Checked the svg repo and found out that the current version is '0.4.0'
    - So back to the `package.json` & `package-lock.json`. I went into those files and just added the `4`. 
    - Fixed that one issue at least. 
    
    

Still having issues with it. Tried `npm run dev` and it's still giving me this error. But this one I'm not sure how to fix.


   ![newError](https://user-images.githubusercontent.com/97326786/156517356-a369c001-f877-495e-a550-8bc5f43d02d9.png)

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Special Directories

You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

### `assets`

The assets directory contains your uncompiled assets such as Stylus or Sass files, images, or fonts.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

### `components`

The components directory contains your Vue.js components. Components make up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/components).

### `layouts`

Layouts are a great help when you want to change the look and feel of your Nuxt app, whether you want to include a sidebar or have distinct layouts for mobile and desktop.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts).

### `pages`

This directory contains your application views and routes. Nuxt will read all the `*.vue` files inside this directory and setup Vue Router automatically.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/get-started/routing).

### `plugins`

The plugins directory contains JavaScript plugins that you want to run before instantiating the root Vue.js Application. This is the place to add Vue plugins and to inject functions or constants. Every time you need to use `Vue.use()`, you should create a file in `plugins/` and add its path to plugins in `nuxt.config.js`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins).

### `static`

This directory contains your static files. Each file inside this directory is mapped to `/`.

Example: `/static/robots.txt` is mapped as `/robots.txt`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/static).

### `store`

This directory contains your Vuex store files. Creating a file in this directory automatically activates Vuex.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/store).
