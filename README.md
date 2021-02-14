# Calvin Abstraction Website
A [Hugo](https://gohugo.io) implementation of the [Calvin Abstraction Website](https://abs.calvin.edu/).

## Getting Started: Updating Website Content
If you plan to update the website content, it is not required to setup a development environment. Rather, you can directly edit the files ending in .md from within Github and benefit from the continuous deployment. 
However, if you wish to create new posts or pages; or restructure the website, you'll need to setup a development environment.

## Getting Started: Setting up a Local Environment
If you are interested in changing the theme or checking under the hood of the website, follow these instructions.

### Prerequisites
Before working on the website, you will need:
* [Hugo Installed](https://gohugo.io/getting-started/installing/) and [git](https://git-scm.com/downloads) (to install a Hugo submodule theme).
* Know basic git commands: clone, staging/commiting, managing/pushing to remotes.
### Instructions
A.
1. Clone repo and ensure the theme installs
```
git clone --recurse-submodules git@github.com:Calvin-Abstraction/Calvin-Abstraction.github.io.git
```
If already cloned,
```
git submodule update --init --recursive
```
2. Run the Hugo server
```
hugo server -D
```
### Create New Page
To create a normal "webpage", add the name of the page in the content/ directory. Ex:
```
cat > content/[insert-new-page-name].md
+++
title = "[insert-new-page-name]"
type = "page"
+++
```
Use Ctrl-D to stop writing to the file.

### Creating New Blog Post
To create a blog post with some metadata generated (such as the current timestamp), run:
```
hugo new posts/my-new-post.md
```

