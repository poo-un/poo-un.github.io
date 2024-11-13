# POO-UN Website

This repository contains the source code for the POO-UN GitHub Pages website, built with [Hugo](https://gohugo.io/).

## Prerequisites

Make sure you have [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) installed on your system.

## Installation

Clone the repository and update Hugo modules:

```bash
git clone https://github.com/poo-un/poo-un.github.io
cd poo-un.github.io
hugo mod get -u
```

## Making Edits

Edit / create content files as needed.

## Running Locally

To preview your changes, start the local server:

```bash
hugo server --buildDrafts --disableFastRender
```

Visit [http://localhost:1313/](http://localhost:1313/) in your browser to see the site.

## Deployment

When ready to publish, commit and push your changes:

```bash
git commit -am 'my great updates'
git push
```