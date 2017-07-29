###File Structure
----

Note: Highlighting the most relevant folders/files below. 

- [.meteor](#meteor)
	- [packages](#packages)
- [client](#client)
    - [css](#css)
    	- [style.scss](#stylescss)
    - [layouts](#layouts)
    - [libs](#libs)
    - [templates](#templates)
    - [head.html](#headhtml)
- [i18n](#i18n)
	- en.i18n.json
	- es.i18n.json
- [lib](#lib)
    - collections.js
    - routes.js
- [private](#private)
- [public](#public)
	- /images
- [server](#server)
- [.gitignore](#gitignore)
- [CODE_OF_CONDUCT.md](#codeofconduct)
- [README.md](#readme)
- [settings-development.json](#settings-development)

## .meteor <a name="meteor"></a>

### /packages <a name="packages"></a>
Contains a list of all meteor packages installed for the app. 

The ones that have a `:` (e.g. twbs:boostrap) mean that they are third-party packages. 

Packages like `check@1.2.5` and `ejson@1.0.13` mean they are native Meteor packages.

You can search for meteor packages on [https://atmospherejs.com](https://atmospherejs.com).

## client <a name="client"></a>
Contains the client-side code.

### css <a name="css"></a>
We use SASS. If you want to create a new SASS file, name it '_yourfile.scss' and be sure to `@import` it in style.scss. 

For a quick introduction to SASS, please read [http://sass-lang.com/guide](http://sass-lang.com/guide).

## i18n <a name="i18n"></a>
Contains the dictionary for keywords defined throughout the app. 

You'll find use case examples sprinkled throughout the HTML files underneath `client/templates`. They follow a bracket format with an underscore at the begininng, like `{{_ "keyword"}}`. 

For example, ```<h4 class="modal-title text-center">{{_ "start_a_hangout"}}</h4>``` on line 6 in  `client/templates/hangout/hangout-clone.html` points to `  "start_a_hangout": "Start a Hangout",` on line 24 in `i18n/en.i18n.json`. 

So the meteor app will render `{{_ "start_a_hangout"}}` as "Start a Hangout" text on the front-end. 

The "Start a hangout" text appears on multiple buttons throughout the website; if we ever wanted to change this text globally, we'd only need to tweak the `i18n/en.i18n.json` file.

=== 

es.i18n.json contains Spanish translations. 

## lib <a name="lib"></a>
Key files in here: collections.js (defines all the collections) and routes.js (defines the routes).

## private <a name="private"></a>
Contains email notification HTML tempaltes and the meta tags for SEO.

## public <a name="public"></a>
Contains the `images` directory.

## server <a name="server"></a>
Contains server-side javascript code, including publications.

## .gitignore <a name="gitignore"></a>
All the files we don't want to push.

## CODE_OF_CONDUCT <a name="codeofconduct"></a>
Code of Conduct for the project.

## README.md <a name="readme"></a>
README for the project.

## settings-development.json <a name="settings-development"></a>
This file holds the settings you're running when you type `meteor --settings settings-development.json` to run the app. Note that it contains dev (not production) API keys.
