# lockfile-shaker-strapi

Plugin for [`lockfile-shaker`](https://github.com/arrowheadapps/lockfile-shaker) that provides configuration for [Strapi](https://github.com/strapi/strapi) serverless deployments.

This has only been tested for Strapi v3.6.10. Use at your own risk for other Strapi versions.

## Installation

Install `lockfile-shaker` and `lockfile-shaker-strapi` (as a dev-dependency):

```
npm i -D lockfile-shaker lockfile-shaker-strapi
```

Add `lockfile-shaker` to your postinstall script:

```JSON
{
  "scripts" : {
    "postinstall": "lockfile-shaker"
  }
}
```
