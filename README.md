# depu

[![build status][travis-image]][travis-url]

automatically update dependencies of your NodeJS application

## Usage

```bash
npx depu [--major|minor|patch] [--prefix="@myNamespace"]
```

depu will
* look for outdated packages (`npm outdated`)
* look for available versions (`npm view myPackage version`)
* install newer packages with `npm install myPackage@1.2.3` which also updates the package.json
* commit the updated package.json and package-lock.json (`git commit -m "updated dependencies`)

## License

MIT

[travis-image]: https://img.shields.io/travis/bseber/depu.svg?style=flat-square
[travis-url]: https://travis-ci.org/bseber/depu
