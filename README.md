# Start [Docusaurus][]

[Docusaurus]: https://github.com/facebook/docusaurus

[![Status](https://img.shields.io/badge/Docusaurus-v2-brightgreen)](https://github.com/facebook/docusaurus)

* [Start online demo](https://ikuokuo.github.io/start-docusaurus2/) 👀
* [Docusaurus offical docs](https://v2.docusaurus.io/docs/)

---

## Installation

### Requirements

* Node.js version >= 10.15.1
* Yarn version >= 1.5

```zsh
❯ node -v
v12.18.4

❯ yarn version
yarn version v1.22.10
```

### Scaffold project website

```zsh
# npx @docusaurus/init@latest init [name] [template]
npx @docusaurus/init@latest init my-website classic
```

Result:

```zsh
Success! Created my-website
Inside that directory, you can run several commands:

  yarn start
    Starts the development server.

  yarn build
    Bundles the app into static files for production.

  yarn deploy
    Publish website to GitHub pages.

We suggest that you begin by typing:

  cd my-website
  yarn start

Happy hacking!
```

### Running the development server

```zsh
cd my-website/
yarn start
```

Visit http://localhost:3000/start-docusaurus2/ .

## Deployment

### Deploying to [GitHub Pages][]

[GitHub Pages]: https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/about-github-pages#about-github-pages

Modify `docusaurus.config.js`:

```js
module.exports = {
  title: 'My Site',
  tagline: 'The tagline of my site',
  url: 'https://ikuokuo.github.io',
  baseUrl: '/start-docusaurus2/',
  onBrokenLinks: 'throw',
  favicon: 'img/favicon.ico',
  organizationName: 'ikuokuo',
  projectName: 'start-docusaurus2',
  ...
};
```

Deploy:

```zsh
cd my-website/
GIT_USER=ikuokuo USE_SSH=true yarn deploy
```

Visit https://ikuokuo.github.io/start-docusaurus2/ .

<!--
❯ vi ~/.ssh/config
Host github.com
  HostName github.com
  User ikuokuo
  PreferredAuthentications publickey
  IdentityFile ~/.ssh/ik_rsa
-->
