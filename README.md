# rfrost-xyz

Website source files for personal website/blog. Continuously deployed to the Netlify, and hosted at [https://rfrost.xyz](https://rfrost.xyz)

## Usage

### Pre-requisites
* [Hugo](https://gohugo.io/getting-started/installing/) (0.84.3, or above)

### Preview locally
Once running, you will be able to preview the locally hosted version at [localhost:1313](http://localhost:1313/).

```shell
hugo serve
```

### Continuous deployment to Netlify

[![Netlify Status](https://api.netlify.com/api/v1/badges/639fb7a9-1d1a-40b2-9286-1d2163e8965e/deploy-status)](https://app.netlify.com/sites/rfrost-xyz/deploys)

Framework for automatic deployment to [Netlify](https://www.netlify.com) is [setup](netlify.toml) whenever the `main` branch on [this repository](https://github.com/rdfrost/rfrost-xyz) receives a push.