# asdf-io

[![Travis](https://img.shields.io/travis/mracos/asdf-io.svg?style=flat-square)](https://travis-ci.org/mracos/asdf-io)

[Io](http://iolanguage.org/) plugin for [asdf](https://github.com/asdf-vm/asdf) version manager.

## Install

```
asdf plugin-add io https://github.com/mracos/asdf-io.git
```

## Use

Check [asdf](https://github.com/asdf-vm/asdf) readme for instructions on how to install & manage versions of Io.

## Eerie :warning:

By default it does not build with the [eerie](https://github.com/IoLanguage/eerie) package manager because of different compilation process for versions before (2019.05.22-alpha).


## Addons
By default it does not build with the addons either, but you can pass a `WITH_IO_ADDONS` env var to the install command, e.g.
`WITH_IO_ADDONS=true asdf install io $VERSION`

:warning: for versions after (`2019.05.22-alpha`) the addons are now eerie packages, so the flag above will not work

please see [IoLanguage/io#400](https://github.com/IoLanguage/io/issues/400) for more information

Keeping in mind that you'll need the following packages if building with the addons
- [yajl](https://github.com/lloyd/yajl)
- [libevent](http://libevent.org/)
- [pcre](http://www.pcre.org/)
- [memcached](https://memcached.org/)
- [ode](http://www.ode.org/)
- [sqlite](http://www.sqlite.org/)
