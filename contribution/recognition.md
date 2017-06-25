#### Recognition as a contributor
-----
Submitted your PR? Congratulations! There are two places you should add yourself as a contributor: README.md, and the [codebuddies.org/about](http://codebuddies.org/about) page.

First:

* Switch to the `adding-contributor` branch.
  * `git checkout adding-contributor`
* Merge the latest changes into this branch.
  * `git merge staging`

#### README.md
  * Open `readme.md` in your editor of choice.
  * Go to [How do I contribute to this project?](/readme.md#how-do-i-contribute-to-this-project) in the readme
  * Add your GitHub handler, GitHub profile page, and what you worked on _above the line "Add Your Name Above"_
    * example: `@Example, https://github.com/onlyforexample - provided an example on Contributing.md`
  * Commit your changes

#### [ABOUT](http://codebuddies.org/about) page
  * Open `client/templates/other/about.html` in your editor of choice
  * Add the following code above the comment "Add Your Name Above!" (NB: Best to `cmd + f` this line.):

```html
<a rel="popover" class="user-popover" title="ADD_SLACK_HANDLER_HERE
  <a href='ADD_TWITTER_LINK_HERE'><i class='fa fa-twitter'></i></a>
  <a href='ADD_GITHUB_LINK_HERE'><i class='fa fa-github'></i></a>
  <a href='ADD_PERSONAL_SITE_HERE'><i class='fa fa-link'></i></a>"  
  data-content="ADD INFORMATION ABOUT YOU AND HOW YOU CONTRIBUTED TO CODEBUDDIES" data-placement="top" data-toggle="popover">
  <img src="ADD_IMG_URL_HERE" class="img-circle" alt="YOUR_NAME"/>
</a>
```
  * Replace the following values:
    * **ADD_SLACK_HANDLER_HERE** - replace with your Slack handler (e.g., @sample)
    * **ADD_TWITTER_LINK_HERE** - replace with your Twitter link
      * If you don't have a Twitter account, delete `<a href='ADD_TWITTER_LINK_HERE'><i class='fa fa-twitter'></i></a>`
    * **ADD_GITHUB_LINK_HERE** - replace with your GitHub link
    * **ADD_PERSONAL_SITE_HERE** - replace with your actual site
      * If you don't have a personal site, delete `<a href='ADD_PERSONAL_SITE_HERE'><i class='fa fa-link'></i></a>`
    * **ADD INFORMATION ABOUT YOU AND HOW YOU CONTRIBUTED TO CODEBUDDIES** - replace this with the requested information!
    * **ADD_IMG_URL_HERE** - replace with a image URL of yourself! (Can be your GitHub profile picture.)
  * Commit and push your changes!

#### Submit a PR
* [Submit a PR](https://help.github.com/articles/creating-a-pull-request/)! (You may link it to your issues' PR, so the code reviewer can review your contributor additions as well.)
* **Remember not to delete this branch, so that others can use the `adding-contributor` as well**
