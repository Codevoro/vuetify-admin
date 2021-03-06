<p align="center">
<a href="https://www.okami101.io/vuetify-admin" target="_blank" rel="noopener"><img src="docs/.vuepress/public/logo.svg" width="300"></a>
</p>

<p align="center">
<a href="https://www.npmjs.com/package/vuetify-admin"><img src="https://img.shields.io/npm/v/vuetify-admin.svg?style=flat-square" alt="Latest Version on NPM"></a>
<a href="https://www.npmjs.com/package/vuetify-admin"><img src="https://img.shields.io/npm/l/vuetify-admin.svg?style=flat-square" alt="License"></a>
</p>

# Vuetify Admin

SPA Admin Framework for **Vue.js** running on top of **REST APIs**, built on **Vuetify** and comes with dedicated [Vue CLI plugin](https://www.npmjs.com/package/vue-cli-plugin-vuetify-admin) for 🚀. Ready to use on **Laravel 8** by using official [Laravel Admin](https://github.com/okami101/laravel-admin) composer package, but can be used on every backend of your choice with your own data and authentication providers.

> See [full documentation](https://www.okami101.io/vuetify-admin)  
> Check [online demo](https://va-demo.okami101.io) -> go to admin and use pre-filled login (read only)  
> Check [tutorial CodeSandbox](https://codesandbox.io/s/github/okami101/vuetify-admin/tree/master/examples/tutorial) -> use any login (fake writeable API)  
> This project was heavily inspired by [React Admin](https://github.com/marmelab/react-admin/) made by awesome [Marmelab Team](https://marmelab.com/)

[![demo](docs/.vuepress/public/assets/screenshot.png)](https://va-demo.okami101.io)

## Features

* Powered by **[Vuetify](https://vuetifyjs.com/)**.
* 🔌 Full standalone **responsive SPA Admin UI** that can be adapted to **any backend (REST, GraphQL, SOAP, etc.)** by writing your **own [data](https://www.okami101.io/vuetify-admin/guide/data-providers.html#writing-your-own-data-provider) and [auth](https://www.okami101.io/vuetify-admin/guide/authentication.html#writing-your-own-auth-provider) providers** by following specific contracts which ensure compatibility.
* ⚡ Bare **minimal Vue.js boilerplate code** needed to get your CRUD pages working via [DSL](https://en.wikipedia.org/wiki/Domain-specific_language) approach.
* 🚀 [Vue CLI plugin](packages/cli) provided for **[immediate quick start](https://www.okami101.io/vuetify-admin/guide/getting-started.html)** while including nice [material theme by Creative Tim](https://github.com/creativetimofficial/vuetify-material-dashboard). Can be used on any Vue.js based application as well.
* 💝 100% **Vue CLI friendly**. The Vuetify Admin library is simply a plugin which integrates within all of your existing plugins, notably **Vue Router, Vuex, Vue I18n and Vuetify**. Keep total control of your Vue app by adding your own routes with **custom pages, custom store modules, and Vuetify theme** as you are used to on Vue CLI base project.
* 👓 [Bookstore demo](https://va-demo.okami101.io/) application which made use of all Vuetify Admin features.
* 🗄 [Complete documentation](https://www.okami101.io/vuetify-admin).
* 🚀 Many tutorials for quick starting with [JSON Server](https://www.okami101.io/vuetify-admin/guide/tutorial.html), [Symfony API Platform](https://www.okami101.io/vuetify-admin/guide/api-platform.html), and [Laravel](https://www.okami101.io/vuetify-admin/guide/laravel.html).
* Ready to use [data providers](https://www.okami101.io/vuetify-admin/guide/data-providers.html) for Laravel within [Spatie Laravel query builder](https://github.com/spatie/laravel-query-builder), hydra for [API Platform](https://api-platform.com/) and [JSON Server](https://github.com/typicode/json-server).
* 🚀 Official separate [Laravel Admin](https://github.com/okami101/laravel-admin) package provided for **insane quick start from top to bottom**. Provides many backend features as spa authentication, profile editing, users management, impersonation, [translatable fields](https://github.com/spatie/laravel-translatable), [media support](https://github.com/spatie/laravel-medialibrary), [file manager](https://github.com/Studio-42/elFinder) with Wysiwyg bridges, etc.
Allow immediate start development from backend to UI with already basic functional admin.
* 🔒 3 [auth providers](https://www.okami101.io/vuetify-admin/guide/authentication.html) included : the recommended **cookie based authentication** for [Laravel Sanctum](https://github.com/laravel/sanctum), **stateless authentication with JWT** (tested with [Laravel JWT](https://github.com/tymondesigns/jwt-auth)), and simple **basic HTTP auth**.
* 🔒 Simple **guest authentication support** if no auth provider transmitted.
* ⛔ Advanced **[user permissions helpers](https://www.okami101.io/vuetify-admin/guide/authorization.html)** for hide/show some UI components or menu links.
* Stay as little magic as possible by fully respecting each backend and frontend development environnement. If you know well Laravel and Vue CLI basics, so you're ready to go !
* 🚀 Automatic **[guesser CRUD pages](https://www.okami101.io/vuetify-admin/guide/getting-started.html#at-a-glance)** which print full Vue.js template generated code as starter kit for your own templates.
* 🚀 **[CRUD code generator commands](https://www.okami101.io/vuetify-admin/guide/generators.html)** on both Laravel and Vue CLI for even quicker ready-to-go API and UI base code.
* ⚡ With usage of Vuetify Admin, code generators as well as Vue.js power, feel the **better mix between productivity, nice development experience and limitless customization**.
* 📝 Full intellisense support for all VA Components on **Vetur and Jetbrains products** !
* 🌍 **[Internationalization support](https://www.okami101.io/vuetify-admin/guide/i18n.html)** via Vue I18n, include english and french translations. Can be easily configured by taking user browser language.
* 🌍 **[Translatable resource fields](https://www.okami101.io/vuetify-admin/guide/i18n.html#resource-translation)** by contextual language selection on each crud page.
* Full **[composable layout](https://www.okami101.io/vuetify-admin/guide/crud/layout.html)** support, with replaceable AppBar, Header, Footer, Sidebar and Aside regions.
* 3 **providers component** for minimal boilerplate code : **[list](https://www.okami101.io/vuetify-admin/guide/crud/list.html), [show](https://www.okami101.io/vuetify-admin/guide/crud/show.html) and [form](https://www.okami101.io/vuetify-admin/guide/crud/form.html)**.
* Many [fields](https://www.okami101.io/vuetify-admin/guide/components/fields.html) and [inputs](https://www.okami101.io/vuetify-admin/guide/components/inputs.html) components for various data types: **select, boolean, number, rich text**, etc.
* **[Server-side form validation](https://www.okami101.io/vuetify-admin/guide/crud/form.html#server-side-validation)** support.
* **[Autocomplete](https://www.okami101.io/vuetify-admin/guide/components/inputs.html#autocomplete)** input with entity reference support.
* **[TinyMCE 5](https://www.okami101.io/vuetify-admin/guide/components/inputs.html#rich-text)** as default Wysiwyg with **elFinder bridge**, can be replaced by your own.
* Create your **own [fields](https://www.okami101.io/vuetify-admin/guide/components/fields.html#custom-component) and [inputs](https://www.okami101.io/vuetify-admin/guide/components/inputs.html#custom-component)** simply by extending mixins.
* [Full-featured DataTable](https://www.okami101.io/vuetify-admin/guide/crud/list.html#data-table), including **multi-sort, pagination, global search, [advanced filters](https://www.okami101.io/vuetify-admin/guide/crud/list.html#advanced-filters), [basic CSV export](https://www.okami101.io/vuetify-admin/guide/crud/list.html#export), live query string context**. And of course with possibility of **[cell templating](https://www.okami101.io/vuetify-admin/guide/crud/list.html#field-templating)**.
* [Data iterator](https://www.okami101.io/vuetify-admin/guide/crud/list.html#data-iterator) decoupled from data table which allows **[total customization of list layout](https://www.okami101.io/vuetify-admin/guide/crud/list.html#custom-layout)**.
* 🔍 Advanced **[as-you-type filters](https://www.okami101.io/vuetify-admin/guide/crud/list.html#advanced-filters)** with many supported inputs: select, boolean, autocomplete for search by relations, with multiple, etc.
* [Bulk actions](https://www.okami101.io/vuetify-admin/guide/crud/list.html#bulk-actions) support.
* Customizable by-row, bulk and global actions.
* Possibility of direct **[aside create/edit](https://www.okami101.io/vuetify-admin/guide/crud/list.html#aside-usage-sample)** from list instead of separate crud page for simple forms.
* 🍻 Support of resources **[associations](https://www.okami101.io/vuetify-admin/guide/crud/list.html#associations)** for relationships.
* Support of **[row editable form](https://www.okami101.io/vuetify-admin/guide/crud/list.html#editable-rows)** on data table for quick creation and edition.
* Support of **[fully editable Treeview](https://www.okami101.io/vuetify-admin/guide/crud/list.html#treeview)** for hierarchical data with drag & drop feature.
* 🤑 To finish, for what it's worth, it's completely **free of charge**.

## Disclaimer

As this project was entirely made on my personal free time while I'm employed, and is totally free of charge, don't expect any support of anything. This project only aims to satisfy my own needs on personal projects for now.

This is a alpha version, without any unit tests or CI yet, so probably plenty of 🐛. Expect regular breaking changes 💥. Mainly for adventurers !

If you look for a free SPA admin library with good support and large community, I strongly encourage you to go with [React Admin](https://github.com/marmelab/react-admin/) which is far more mature, optimized and fully tested. On commercial side you should take a look to [Laravel Nova](https://nova.laravel.com/) for highest productivity with nice SPA UI. For more classical and free efficient admin builder take a look on [EasyAdmin](https://github.com/EasyCorp/EasyAdminBundle).

## Architecture

![Architecture](docs/diagrams/architecture.svg)

> See how it works [here](https://www.okami101.io/vuetify-admin/guide/#how-it-works).

## Install

Select your most suitable guide :

* For basic presentation and quick install via the Vue CLI Plugin, go to [getting started](https://www.okami101.io/vuetify-admin/guide/getting-started.html).
* For best initial starting showcase of Vuetify Admin features, follow [this tutorial guide](https://www.okami101.io/vuetify-admin/guide/tutorial.html).
* If you choose Laravel as backend, follow [this optimized guide](https://www.okami101.io/vuetify-admin/guide/laravel.html).

## Note on this main repo

It's contains all necessary projects to develop Vuetify Admin and run demo and tutorials :

* [Vuetify Admin Library](packages/admin), the main admin library.
* [Vuetify Admin Vue CLI Plugin](packages/cli), the associated Vue CLI plugin which contains all base code boilerplate for quick install and UI commands code generator.
* [Laravel Admin](https://github.com/okami101/laravel-admin), git submodule of composer package to use on fresh Laravel project which facilitates Vuetify Admin integration and includes server-side API commands generator.
* [Bookstore Admin Demo](examples/demo), full-featured admin sample build on top of main Vuetify Admin Library.
* [Bookstore Laravel Demo](examples/demo-laravel), suitable API backend for bookstore admin demo based on Laravel.
* [Admin Tutorial](examples/tutorial), finished tutorial after following [dedicated docs](https://www.okami101.io/vuetify-admin/guide/tutorial.html), ideal for quick learning in less than 15 minutes.
* [API Platform Tutorial](examples/api-platform), finished tutorial after following [dedicated docs](https://www.okami101.io/vuetify-admin/guide/api-platform.html). Good showcase of hydra API provider usage.
* [Laravel Tutorial](examples/laravel), finished tutorial after following [dedicated docs](https://www.okami101.io/vuetify-admin/guide/laravel.html) which aims to made a good showcase of YAML driven development.
* [Vue CLI base](vue-cli-base), clean basic Vuetify CLI project starter for proper install testing of [VA Vue CLI plugin](packages/cli).
* [Docs](docs), documentation based on VuePress.

> All of this projects are automatically linked together by symlinks thanks to yarn workspaces and composer for best library development experience. HMR from demo to admin library side-by-side is fully supported !

## Usage

### How to run tutorial

You can run tutorial directly inside [CodeSandbox](https://codesandbox.io/s/github/okami101/vuetify-admin/tree/master/examples/tutorial) !

### How to run demo locally

Be sure to have cloned this repo with git submodules. If not the case use `git submodule init && git submodule update`. [The separate Laravel package](https://github.com/okami101/laravel-admin) should be cloned under **packages/laravel** sub folder.

Requirements :

* **Yarn**.
* **Docker** with **docker-compose**, required for quick-start run backend API. If you don't want it, follow [dedicated instructions](examples/demo-laravel#classic).
* **Make** for easy starting all necessary tools. For Windows users install it via [scoop](https://scoop.sh/) with `scoop install make`. Use `make help` for all detail commands.

In order to run demo :

```bash
yarn # install all yarn dependencies
make up-demo-laravel # run server api through docker (take a pastis if 1st time...)
make prepare-demo-laravel # initialize laravel app and inject dummy data (use it only at 1st launch)
make run-demo # compile all bookstore demo admin with HMR dev mode enabled
```

Admin panel should autostart at [http://localhost:8080](http://localhost:8080).

### Run and build docs

Docs are hosted by VuePress. Use `make run-docs` to launch it on [http://localhost:9000](http://localhost:9000). `make build-docs` will generate static files inside `docs` root folder.

> API documentation for all VA components are auto generated from source code thanks to [Vue Docgen API](https://vue-styleguidist.github.io/docs/Docgen.html).

### Laravel Admin

A [separate helper package](https://github.com/okami101/laravel-admin) is available for Laravel in order to have the quickest starting development experience as possible, combined to generators for high productivity, while highly respecting the pure traditional Laravel way to make CRUD resources. I included YAML based code generators, similarly as [Blueprint](https://github.com/laravel-shift/blueprint).

## Documentation

Documentation for Vuetify Admin can be found on the [Okami101 website](https://www.okami101.io/vuetify-admin).

## License

This project is open-sourced software licensed under the [MIT license](https://adr1enbe4udou1n.mit-license.org).
