### Proof of concept

This is a proof of concept to see if we can use a static page instead of the Wordpress page at piratar.is

Pros:
* No need to update Wordpress, plugins, server etc
* It can be hosted for free on Github. (Serverless)
* User authentication: 
  * No need to create a new user or manage permissions for people needing to edit.
* We can accept changes from *anyone* through pull requests.

Cons:
* We need to learn something new
* We have to sign up for a Github account (free)


### Can we:
- [x] Import the old site? Yes: http://import.jekyllrb.com/docs/wordpress/ (We should test this before going forward!)
- [x] Use themes? Yes,currently using: https://github.com/mmistakes/minimal-mistakes
- [x] Edit permalinks? Yes: https://jekyllrb.com/docs/permalinks/
- [x] Use translations? Yes: https://www.sylvaindurand.org/making-jekyll-multilingual/
- [x] Have a calendar? Yes


### Quick start for development
1. Clone this repo

1. Install jekyll and the theme  
`bundle`

1. Start the dev server. (If the main domain uses a subpath on Github, add `--baseurl ''`)  
`./server.sh` or `bundle exec jekyll serve`

1. Visit [http://localhost:4000](http://localhost:4000)

### Working with Markdown

While editing a page/post we recommend people copy/paste the content to a site like:

* [Dillinger.io](https://dillinger.io/)
* [Hackmd.io](https://hackmd.io/)

And copy the contents back when done. (Until Github supports this side by side workspace)


### Organization of files

* If you are a content creator, you need to learn the basics:

* All blog posts or news should go into the **'_posts'** folder.

* All pages and the correct folder structure (the webtree) goes in the **'_pages'** folder.

* The top menu is defined in `_data/navigation.yml`

* Images go in /assets/images/


### Creating a new page/post

The top of each page or post should have:

```
---
title: Blogging Like a Hacker
---
```

This section is called [Front Matter](https://jekyllrb.com/docs/frontmatter/)


### Themes

Swithcing themes is easy and can be done in the `_config.yml` (or project settings on Github)

We are currently using this theme for testing: https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/


## Useful links

https://devhints.io/jekyll

https://jekyllrb.com/docs/structure/
