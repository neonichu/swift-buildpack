# Heroku buildpack for Swift

[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)

A simple Swift buildpack, uses the official Ubuntu LTS build
from the [Swift website][1].

## Usage

Create a new app using the buildpack:

```bash
$ heroku create -b https://github.com/neonichu/swift-buildpack.git
```

or add it to an existing app:

```bash
$ heroku config:add BUILDPACK_URL=https://github.com/neonichu/swift-buildpack.git
```

All the Swift binaries are installed into `vendor/swift` and are
available via `PATH`.

## Example

This [script][2] might work as an example.


[1]: https://swift.org
[2]: https://gist.github.com/neonichu/c504267a23ca3f3126bb
