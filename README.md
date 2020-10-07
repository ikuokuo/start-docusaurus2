# Start [Docusaurus][]

[Docusaurus]: https://github.com/facebook/docusaurus

[![Status](https://img.shields.io/badge/Docusaurus-v2-brightgreen)](https://github.com/facebook/docusaurus)

* [Offical Docs](https://v2.docusaurus.io/docs/)

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
# npx @docusaurus/init@next init [name] [template]
npx @docusaurus/init@next init my-website classic
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
