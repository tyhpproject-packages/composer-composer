<!-- tyhp-readme:start -->
# tyhpdef/composer-composer

Tyhp type definitions for `composer/composer` `2.10.3`.

```bash
composer require --dev tyhpdef/composer-composer:2.10.3
```

This is a metapackage. Composer also installs `tyhpdef/composer-composer-impl` (type files).
Require **this** name, not `tyhpdef/composer-composer-impl`.

See https://tyhplang.com.

## Maintain `composer/composer`? Ship the types yourself

If you are a Packagist maintainer of `composer/composer`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/composer-composer-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `composer/composer` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/composer-composer": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `composer/composer` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `composer/composer` with a real constraint,
   `"replace": { "tyhpdef/composer-composer": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `composer/composer` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/composer-composer` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
