#### Dear Adalyte,

You are encouraged to participate in the Lair’s Blog.

To contribute, clone this GIT repository to your machine.
Add your profile to the folder `_data/authors/`. You can use Chas’ profile in `_data/authors/chasnelson.yml` as a template. The name of the file will be your username on the website. This username is only used to attribute blog posts the right person but it is not otherwise visible.

Put your picture in the folder `assets/images/authors/`. Your picture should be square due to a limitation of the current CMS otherwise you will look horribly disfigured on the website.

You can write new blog posts in the `_posts` directory. The filename should have the format `year-month-day-your-title.md` to be properly indexed and start with

```markdown
---
author: your-username
---
```

You can have a look to other posts and to [Github’s Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) and to [Jekyll’s documentation](https://jekyllrb.com/docs/posts/) for more information on how to write new posts.

To make your changes visible, commit and push your changes. The website will be automatically updated.


Yours sincerely,

#### PS:
You can also host a local copy of the website to test your changes before pushing them. To do so, install Bundler on your system and the required dependencies by running in the repository’s root directory:

```bash
sudo apt-get install bundler
bundle install
```

Then everytime that you want to to test, run the following command

```bash
export PATH=$PATH:$HOME/.gem/ruby/2.4.0/bin # Might be needed on your system
bundle exec jekyll serve
```

and open the page [http://localhost:4000](http://localhost:4000). If you make any modification to your post while Jekyll is running, just reload your page after a couple of seconds and the changes will appear automatically.

#### PPS:
If you were to modify the Javascript code of the blog. You need to regenerate the minified version. To do so install npm and the required dependencies by running in the repository’s root directory:

```bash
apt-get install npm
npm install
```

Then everytime needed:

```bash
npm run build:js
```

