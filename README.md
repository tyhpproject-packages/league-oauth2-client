<!-- tyhp-readme:start -->
# tyhpdef/league-oauth2-client

Tyhp type definitions for `league/oauth2-client` `2.9.1`.

```bash
composer require --dev tyhpdef/league-oauth2-client:2.9.1
```

This is a metapackage. Composer also installs `tyhpdef/league-oauth2-client-impl` (type files).
Require **this** name, not `tyhpdef/league-oauth2-client-impl`.

See https://tyhplang.com.

## Maintain `league/oauth2-client`? Ship the types yourself

If you are a Packagist maintainer of `league/oauth2-client`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/league-oauth2-client-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `league/oauth2-client` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/league-oauth2-client": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `league/oauth2-client` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `league/oauth2-client` with a real constraint,
   `"replace": { "tyhpdef/league-oauth2-client": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `league/oauth2-client` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/league-oauth2-client` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
