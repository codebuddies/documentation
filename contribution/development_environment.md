#### Setting Up Your Development Environment
----

1. Install Meteor. On a mac, you should use this command:

   `curl "https://install.meteor.com/?release=1.6.1.1" | sh`
   - On Windows, you should run the official installer [here](https://www.meteor.com/install).
   - If you're unsure whether you already have meteor installed, type `meteor --version` in your command line to check. You should see that you have meteor version 1.3.2.4.

2. Go to [https://github.com/codebuddies/codebuddies](https://github.com/codebuddies/codebuddies). Fork this repository!
  - Click on  "Fork" near the upper right.

4. Once you have a copy of this repo on your own account, clone this repo to your computer by typing in something like:
   `git clone https://github.com/[Your URL Path here]/codebuddies.git`
  - Replace the URL with your own repository URL path.
  - You can also get the above link to clone the repo by going to the github page for your fork of the repo and clinking "Clone or download."

5. Type `cd codebuddies` in your terminal. Then, set up this repository as an upstream branch by typing:
  `git remote add upstream https://github.com/codebuddies/codebuddies.git`

6. Type `meteor npm install` to install the initial meteor packages. You have to do this once!

Now, whenever you want to sync with the owner repository, you can do the following:
  - `git fetch upstream`
  - `git checkout staging`
  - `git merge upstream/staging`

  Note: You can type `git remote -v` to check which repositories your `origin` and `upstream` are pointing to.





#### Start up the App
----

Run `meteor --settings settings-development.json` in your terminal to start up the app in your browser ([http://localhost:3000](http://localhost:3000)). Note that the first time you do this, it may take a while (a few minutes) for the app to start up.

#### (OPTIONAL) How to log in as an admin on localhost:3000

1. Add your email and username to ```settings-development.json```, for the `root_email` and `root_username` keys.
2. ```meteor reset && meteor --settings settings-development.json``` to reset your local database and restart the app.
3. You will receive your password in your email. Note: please check spam filters if you don't see it! Or ask on the #cb-code channel on Slack for a new Sparkpost API key.
4. Go to ```http://localhost:3000/admin``` to log in.

Note: When you create a hangout in localhost:3000, a Slack notification will be sent to the #codebuddies-ops channel. This emulates what happens when you create a hangout on codebuddies.org, where a Slack announcement about the hangout will appear in the #general channel.

#### Notes

* `meteor npm run meteor:dev` can also run the app, but may [use up your CPU](https://github.com/meteor/meteor/issues/4314).

* Also note: if you see an error in your terminal asking you to `meteor npm install --save faker`, please run that command!

* When you create a hangout in your localhost:3000, a Slack notification will be sent to the #codebuddies-ops channel. This emulates what happens when you create a hangout on codebuddies.org, where a Slack announcement about the hangout will appear in the #announcements channel.
