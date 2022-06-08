# lockfile-shaker-strapi

[![NPM Version](https://img.shields.io/npm/v/lockfile-shaker-strapi/latest)](https://www.npmjs.org/package/lockfile-shaker-strapi)
[![Monthly download on NPM](https://img.shields.io/npm/dm/lockfile-shaker-strapi)](https://www.npmjs.org/package/lockfile-shaker-strapi)
[![Snyk Vulnerabilities](https://img.shields.io/snyk/vulnerabilities/npm/lockfile-shaker-strapi)](https://snyk.io/test/npm/lockfile-shaker-strapi)
[![GitHub last commit](https://img.shields.io/github/last-commit/arrowheadapps/lockfile-shaker-strapi)](https://github.com/arrowheadapps/lockfile-shaker-strapi)

Plugin for [`lockfile-shaker`](https://github.com/arrowheadapps/lockfile-shaker) that provides configuration for [Strapi](https://github.com/strapi/strapi) serverless deployments.

This has only been tested for Strapi v3.6.10. Use at your own risk for other Strapi versions.

## Installation

Install `lockfile-shaker` and `lockfile-shaker-strapi` (as a dev-dependency):

```
npm i -D lockfile-shaker lockfile-shaker-strapi
```

Add `lockfile-shaker` to your postinstall script (this will execute `lockfile-shaker` only on `npm install`, not npm `npm ci`):

```JSON
{
  "scripts" : {
    "postinstall": "node -e \"(process.env.npm_command != 'ci') && require('lockfile-shaker/lib/bin.js')\""
  }
}
```
