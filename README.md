# al-folio
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[core_contributors]: https://img.shields.io/badge/core_contributors-3-orange.svg 'Number of core contributors'
<!-- ALL-CONTRIBUTORS-BADGE:END -->

[![deploy](https://github.com/alshedivat/al-folio/actions/workflows/deploy.yml/badge.svg)](https://github.com/alshedivat/al-folio/actions/workflows/deploy.yml)
[![demo](https://img.shields.io/badge/theme-demo-brightgreen.svg)](https://alshedivat.github.io/al-folio/)
[![GitHub contributors](https://img.shields.io/github/contributors/alshedivat/al-folio.svg)](https://github.com/alshedivat/al-folio/graphs/contributors/)
[![Core Contributors][core_contributors]](#core-contributors-)
[![GitHub release](https://img.shields.io/github/v/release/alshedivat/al-folio)](https://github.com/alshedivat/al-folio/releases/latest)
[![GitHub license](https://img.shields.io/github/license/alshedivat/al-folio?color=blue)](https://github.com/alshedivat/al-folio/blob/master/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/alshedivat/al-folio)](https://github.com/alshedivat/al-folio)
[![GitHub forks](https://img.shields.io/github/forks/alshedivat/al-folio)](https://github.com/alshedivat/al-folio/fork)

A simple, clean, and responsive [Jekyll](https://jekyllrb.com/) theme for academics.
If you like the theme, give it a star!


## Getting started

Want to learn more about Jekyll? Check out [this tutorial](https://www.taniarascia.com/make-a-static-website-with-jekyll/).
Why Jekyll? Read [Andrej Karpathy's blog post](https://karpathy.github.io/2014/07/01/switching-to-jekyll/)!


### Installation

For a hands-on walkthrough of al-folio installation, check out [this cool video tutorial](https://www.youtube.com/watch?v=g6AJ9qPPoyc) by one of the community members! 🎬 🍿

#### Local Setup (Standard)

Assuming you have [Ruby](https://www.ruby-lang.org/en/downloads/) and [Bundler](https://bundler.io/) installed on your system (*hint: for ease of managing ruby gems, consider using [rbenv](https://github.com/rbenv/rbenv)*), first [fork](https://guides.github.com/activities/forking/) the theme from `github.com:alshedivat/al-folio` to `github.com:<your-username>/<your-repo-name>` and do the following:

```bash
$ git clone git@github.com:<your-username>/<your-repo-name>.git
$ cd <your-repo-name>
$ bundle install
$ bundle exec jekyll serve
```

Now, feel free to customize the theme however you like (don't forget to change the name!).
After you are done, **commit** your final changes.


If you need to manually re-deploy your website to GitHub pages, run the deploy script from the root directory of your repository:
```bash
$ ./bin/deploy
```
uses the `master` branch for the source code and deploys the webpage to `gh-pages`.

---

