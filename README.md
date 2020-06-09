# gatsby-source-npm-author-packages
## Gatsby source plugin for retrieving NPM Packages by a specific Author

This plugin utilises "libnpmsearch" to find packages on NPM created by a paticular author.

## Install

```
npm i gatsby-source-npm-author-packages
```

## Configure

In `gatsby-config.js`:

```js
    {
      resolve: `gatsby-source-gatsby-source-npm-author-packages`,
      options: {
        author: `npm-author-username`,
      }
    },
```

## Usage 

```graphql
  allNpmPackage {
    nodes {
      version
      name
      links {
        bugs
        homepage
        npm
        repository
      }
      keywords
      description
    }
  }
```

## License

MIT
