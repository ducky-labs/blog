# DuckyLabs Blog

The blog site at https://ducky-labs.github.io/blog is a static site built with Hugo the framework, it is simple yet customisable. Posts are written in markdown and automatically posted to the site when they are no longer marked as drafts.


## Creating a new post

You can create a new post easily using hugo to create new content. Run the below command and edit the markdown file which is created.

```bash
hugo new posts/title-of-post/index.md.md

# Edit the markdown file
nvim content/posts/title-of-post/index.md
```


## Building the site

Hugo is simple, when you are done and have marked all posts which you wish to be published as no longer being drafts you can run one simple command to build the entire site.

```bash
# Build the site
hugo

# Build contents is outputted to public by default
ls -lah public
```


## Deploying the site

The site is automatically built using Github actions and deployed to Github pages now, view the workflow in the `.github/workflows/hugo.yml` file.

```bash
git add .

git commit -m "Updated site"

git push -u origin main
```
