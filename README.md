# Heroku buildpack for Swift

A simple Swift buildpack, uses the official Ubuntu LTS build
from the [Swift website][1].

## Usage

Create a new app using the buildpack:

```bash
heroku create -b https://github.com/neonichu/swift-buildpack.git
```

All the Swift binaries are installed into `vendor/swift` and are
available via `PATH`.

[1]: https://swift.org
