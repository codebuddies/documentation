#### Setting Up Your Development Environment
----
 
2. Install Meteor! On mac, you should use this command: 

   `curl "https://install.meteor.com/?release=1.3.2.4" | sh`

On Windows, you should run the official installer [here](https://www.meteor.com/install). If you're unsure whether you already have meteor installed, type `meteor --version` in your command line to check. You should see that you have meteor version 1.3.2.4.

3. Please star this repository! We need to reach 100 stars so that we can apply to the [Open Collective](https://opencollective.com/opensource/apply).
  [Edit - We're already there! But still star this repo, so others can hear about what we're doing!]
  
4. Fork this repository! Once you have a copy of this repo on your own account, clone this repo to your computer by typing in something like:

  `git clone https://github.com/codebuddiesdotorg/codebuddies.git`

  (Replace the URL with your own repository URL path.)

5. Run `cd codebuddies`. Then, set up this repository as an upstream branch using:
  * `git remote add upstream https://github.com/codebuddiesdotorg/codebuddies.git`

  Now, whenever you want to sync with the owner repository. Do the following:
  * `git fetch upstream`
  * `git checkout staging`
  * `git merge upstream/staging`
  
  Note: You can type `git remote -v` to check which repositories your `origin` and `upstream` are pointing to.

6. Type `meteor npm install` to install the initial meteor packages (you have to do this now, not later when you start up the app!).

You might get errors telling you to run --save to install other packages; please run them:

```
meteor npm install --save babel-runtime
meteor npm install --save faker twitter mailchimp-api body-parser md5
meteor npm install --save jquery lodash uhr quill-render html-to-text
meteor npm install --save bcrypt
meteor npm install 
```



#### Start up the App
----

1. Run `meteor --settings settings-development.json` in your terminal to start up the app in your browser ([http://localhost:3000](http://localhost:3000)). Note that the first time you do this, it may take a while (a few minutes) for the app to start up.
  * (`meteor npm run meteor:dev` can also run the app, but will likely [use up your CPU](https://github.com/meteor/meteor/issues/4314).)
  * Also note: if you see an error in your terminal asking you to `meteor npm install --save faker`, please run that command!
