# DCH Releaser - A Debian's Changelog Bumper

[http://wbotelhos.com/dch_releaser](http://wbotelhos.com/dch_releaser) - DCH Releaser is a script to bump Debian's changelog version.

## Version

```
@version  0.1.0
@since    2014.05.21
@author   Washington Botelho
@doc      wbotelhos.com/dch_releaser
```

## Required Files

+ debian/control

## Options

```bash
major : API changes which are not backward-compatible.
minor : Releases which add new, but backward-compatible, API features.
patch : Minor changes and bug fixes which do not change the software's API.
```

Check [Software Versioning](http://en.wikipedia.org/wiki/Software_versioning) for more information about nomenclature.

## Usage

Given you have a debian's structure files like the following:

```bash
├── debian
│   ├── changelog
│   ├── compat
│   ├── control
│   ├── postinst
│   └── rules
```

```bash
cd project
dch_release option
```

If `changelog` file not exist, then it will be created and the version will be `0.1.0` as the first one.
If `changelog` already exist with some version, this version will be incremented according the option given.

## Plus

You can use the `debian` folder as your template. Just copy it to your project!

## Contributors

[Check it out](http://github.com/wbotelhos/dch_releaser/graphs/contributors)

## Licence

The MIT License

## Love it!

Via [PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=X8HEP2878NDEG&item_name=DCH%20Releaser) or [Gittip](http://www.gittip.com/wbotelhos). Thanks! (:
