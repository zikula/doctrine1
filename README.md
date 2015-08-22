# Doctrine 1 fork

[![Build status](https://travis-ci.org/zikula/doctrine1.svg?branch=master)](https://travis-ci.org/zikula/doctrine1)
[![Total Downloads](https://img.shields.io/packagist/dt/drak/doctrine1.svg)](https://packagist.org/packages/drak/doctrine1)

This is a maintained Doctrine 1 fork you can use in your projects using Composer.

There are two versions: `dev` and `master`.
`master` is fully backwards-compatible with the latest original
Doctrine 1 release. `dev` contains more fixes.

## Usage

Use the `dev-dev` version string for the latest doctrine1,
and `dev-master` for the backwards-compatible one:

```json
{
  "require": {
    "drak/doctrine1": "dev-dev"
  }
}
```

## List of backwards-incompatible changes on `dev`

* `whereIn` with an empty array now restricts query to returning nothing instead of returning
everything ([issue #15](https://github.com/drak/doctrine1/pull/15))
