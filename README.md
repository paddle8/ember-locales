# DEPRECATED

This project will be superceded by a community choice discussed here: https://github.com/yahoo/ember-intl/issues/109. If you have any issues migrating, please provide feedback so we may try to move you nicely into these projects.

# ember-locales

This addon provides internationalization helpers through https://github.com/fnando/i18n-js.

**It requires Ember 1.10+.**

## Getting Started

```bash
ember install:addon ember-locales
```

## Setting up your translation tables

Your translation data lives under `app/locales`. Locales in this folder will be loaded automatically by the addon.

For starters, let's add a translation table for english in the US. We'll call this file 'en-US.js':

```javascript
export default {
  hello: "Hello, %{user}!"
};
```

From here, we can use translation helper in our app:

```handlebars
{{t "hello" user=user.name}}
```

All helpers mirror their JS counterparts. See https://github.com/fnando/i18n-js for more details on how to use helpers.

## Installation

* `git clone` this repository
* `npm install`
* `bower install`

## Running

* `ember server`
* Visit your app at http://localhost:4200.

## Running Tests

* `ember test`
* `ember test --server`

## Building

* `ember build`

For more information on using ember-cli, visit [http://www.ember-cli.com/](http://www.ember-cli.com/).
