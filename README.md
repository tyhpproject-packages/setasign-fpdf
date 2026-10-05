<!-- tyhp-readme:start -->
# tyhpdef/setasign-fpdf

Tyhp type definitions for `setasign/fpdf` `1.9.0`.

```bash
composer require --dev tyhpdef/setasign-fpdf:1.9.0
```

This is a metapackage. Composer also installs `tyhpdef/setasign-fpdf-impl` (type files).
Require **this** name, not `tyhpdef/setasign-fpdf-impl`.

See https://tyhplang.com.

## Maintain `setasign/fpdf`? Ship the types yourself

If you are a Packagist maintainer of `setasign/fpdf`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/setasign-fpdf-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `setasign/fpdf` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/setasign-fpdf": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `setasign/fpdf` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `setasign/fpdf` with a real constraint,
   `"replace": { "tyhpdef/setasign-fpdf": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `setasign/fpdf` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/setasign-fpdf` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
