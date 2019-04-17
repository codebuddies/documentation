# File Structure

### File Structure

Note: Highlighting the most relevant folders/files below.

* [.meteor](index.md#meteor)
  * [packages](index.md#packages)
* [client](index.md#client)
  * [css](index.md#css)
    * [style.scss](index.md#stylescss)
  * [layouts](index.md#layouts)
  * [libs](index.md#libs)
  * [templates](index.md#templates)
  * [head.html](index.md#headhtml)
* [i18n](index.md#i18n)
  * en.i18n.json
  * es.i18n.json
* [lib](index.md#lib)
  * collections.js
  * routes.js
* [private](index.md#private)
* [public](index.md#public)
  * /images
* [server](index.md#server)
* [.gitignore](index.md#gitignore)
* [CODE\_OF\_CONDUCT.md](index.md#codeofconduct)
* [README.md](index.md#readme)
* [settings-development.json](index.md#settings-development)

## .meteor 

### /packages 

Contains a list of all meteor packages installed for the app.

The ones that have a `:` \(e.g. twbs:boostrap\) mean that they are third-party packages.

Packages like `check@1.2.5` and `ejson@1.0.13` mean they are native Meteor packages.

You can search for meteor packages on [https://atmospherejs.com](https://atmospherejs.com).

## client 

Contains the client-side code.

### css 

We use SASS. If you want to create a new SASS file, name it '\_yourfile.scss' and be sure to `@import` it in style.scss.

For a quick introduction to SASS, please read [http://sass-lang.com/guide](http://sass-lang.com/guide).

## i18n 

Contains the dictionary for keywords defined throughout the app.

You'll find use case examples sprinkled throughout the HTML files underneath `client/templates`. They follow a bracket format with an underscore at the begininng, like `{{_ "keyword"}}`.

For example, `<h4 class="modal-title text-center">{{_ "start_a_hangout"}}</h4>` on line 6 in `client/templates/hangout/hangout-clone.html` points to `"start_a_hangout": "Start a Hangout",` on line 24 in `i18n/en.i18n.json`.

So the meteor app will render `{{_ "start_a_hangout"}}` as "Start a Hangout" text on the front-end.

The "Start a hangout" text appears on multiple buttons throughout the website; if we ever wanted to change this text globally, we'd only need to tweak the `i18n/en.i18n.json` file.

===

es.i18n.json contains Spanish translations.

## lib 

Key files in here: collections.js \(defines all the collections\) and routes.js \(defines the routes\).

## private 

Contains email notification HTML tempaltes and the meta tags for SEO.

## public 

Contains the `images` directory.

## server 

Contains server-side javascript code, including publications.

## .gitignore 

All the files we don't want to push.

## CODE\_OF\_CONDUCT 

Code of Conduct for the project.

## README.md 

README for the project.

## settings-development.json 

This file holds the settings you're running when you type `meteor --settings settings-development.json` to run the app. Note that it contains dev \(not production\) API keys.

