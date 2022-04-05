# Gatsbyjs Blog

## Getting started

### Install gatsby

```shell
npm install -g gatsby-cli

```

### Install and start locally:

```shell
gatsby new my-blog https://github.com/zhalice2011/blog
```

### Start the site in develop mode

```shell
cd my-blog
gatsby develop
```

### Open the source code and start editing!

Your site is now running at http://localhost:8000. Open the my-gatsby-site directory in your code editor of choice and edit src/pages/index.js. Save your changes, and the browser will update in real time!


### Deploy to Github Pages

**Step 0**

please replace `zhalice2011` to your github username
```
git remote add origin git@github.com:zhalice2011/zhalice2011.github.io.git
```

**Step 1**

Start by pushing a gh-pages branch. The initial contents of the branch doesn't matter since it will be overridden with the build artifacts on the next step of this guide.

```shell
git checkout -b gh-pages
git push -u origin gh-pages
```

**Step 2**

In `gatsby-config.js`, change the `pathPrefix` to the name of your Github repository

```javascript
module.exports = {
  pathPrefix: `/`,
  ...
}
```

**Step 3**

```shell
npm run deploy
```

If everything goes well, you should be able to access [https://zhalice2011.github.io/](https://zhalice2011.github.io/)


If you set pathPrefix `/blog`
```javascript
module.exports = {
  pathPrefix: `/blog`,
  ...
}
```

you should be able to access [https://zhalice2011.github.io/blog](https://zhalice2011.github.io/blog)