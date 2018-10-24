### Proof of concept

This is a proof of concept to see if we can use a static page instead of the Wordpress page at piratar.is

### Pros:
* No need to update Wordpress, plugins, server etc
* It can be hosted for free on Github. (We don't need to maintain a server)
* User authentication: 
  * No need to create a new user or manage permissions for people needing to edit.
* We can accept changes from *anyone* through pull requests.

### Cons:
* We need to learn something new
* We have to sign up for a Github account (free)


### Can we:
- [x] Import the old site? Yes: http://import.jekyllrb.com/docs/wordpress/ (We should test this before going forward!)
- [x] Use themes? Yes, but now we simply use Bootstrap 4, so more people can easily collaborate. Themes can get complex
- [x] Edit permalinks? Yes: https://jekyllrb.com/docs/permalinks/
- [x] Use translations? Yes: https://www.sylvaindurand.org/making-jekyll-multilingual/
- [x] Have a calendar? Yes


We can do a lot of things, and the best way might be to use an external service and iframe their content into ours.


### Quick start for development
1. Clone this repo

1. Install jekyll and the gems  
`bundle`

1. Start the dev server. (If the main domain uses a subpath on Github, add `--baseurl ''`)  
`./server.sh` or `bundle exec jekyll serve`

1. Visit [http://localhost:4000](http://localhost:4000)

### Working with Markdown

While editing a page/post we recommend people copy/paste the content to a site like:

* [Dillinger.io](https://dillinger.io/)
* [Hackmd.io](https://hackmd.io/)

And copy the contents back when done. (Until Github supports this side by side workspace)


### Organization of files, folder structure

Folder | Usage
------ | ------
\_posts         | Blog posts. Do we need it?
\_pages         | All pages and the correct folder structure (the webtree) goes in the
\_frettir/      | Fréttir (news)
\_data/navigation.yml | Top menu navigation
/assets/images/ | Images


### Creating a new page/post

The top of each page or post should have:

```
---
title: Blogging Like a Hacker
---
```

This section is called [Front Matter](https://jekyllrb.com/docs/frontmatter/)


## Useful links

https://devhints.io/jekyll

https://jekyllrb.com/docs/structure/
