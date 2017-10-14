# [avast.github.io](https://avast.github.io/)

This repository contains the source for [avast.github.io](https://avast.github.io/). It uses GitHub pages with Jekyll templates.

## Adding your repository
Currently, repositories that appear on the page (along with their categories) are listed in the [_config.yml](https://github.com/avast/avast.github.io/blob/master/_config.yml#L5) configuration file. Submit a merge request with your repository added to that file.

Future versions might map displayed categories to certain repository tags, so that repositories show up on the page automatically.

## Changing the template
If you want to tweak the HTML template, follow the instructions in GitHub's [Setting up your GitHub Pages site locally with Jekyll](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/) article (note some of the steps do not apply since you won't need to create the GitHub pages repository from scratch).

Since the current template makes use of [repository metadata](https://help.github.com/articles/repository-metadata-on-github-pages/) in order to display some repository content (description, forks, watchers) dynamically, you'll also need to do some additional token setup as described in the [Using repository metadata locally](https://help.github.com/articles/repository-metadata-on-github-pages/#using-repository-metadata-locally) article.

Then you can run the following command to have the site be regenerated and server locally on every save:

```
JEKYLL_GITHUB_TOKEN=<yourtoken> bundle exec jekyll serve --verbose
```
