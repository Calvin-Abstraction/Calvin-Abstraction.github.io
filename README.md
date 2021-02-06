# Calvin Abstraction Website
A [Hugo](https://gohugo.io) implementation of the [Calvin Abstraction Website](https://abs.calvin.edu/).

## Getting Started: Updating Website Content
If you plan to update the website content, it is not required to setup a development environment. Rather, you can directly edit the files ending in .md from within Github and benefit from the continuous deployment. 

## Getting Started: Website Development
If you are interested in changing the theme or checking under the hood of the website, follow these instructions.

### Prerequisites
Before working on the website, you will need:
[Hugo Installed](https://gohugo.io/getting-started/installing/) and [git](https://git-scm.com/downloads) (to install a Hugo submodule theme).
A.
1. Clone repo and ensure the theme installs
```
git clone --recurse-submodules https://github.com/Calvin-Abstraction/abs-website
```
If already cloned,
```
git submodule update --init --recursive
```
2. Run the Hugo server
```
hugo server -D
```




