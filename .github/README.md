# tc-tap-redirect-builder

[![build](https://github.com/alexellis/tc-tap-redirect-builder/actions/workflows/build.yml/badge.svg)](https://github.com/alexellis/tc-tap-redirect-builder/actions/workflows/build.yml) [![Github All Releases](https://img.shields.io/github/downloads/alexellis/tc-tap-redirect-builder/total.svg)]()

This project is a builder to provide binary releases for [tc-tap-redirect from AWS Labs](https://github.com/awslabs/tc-redirect-tap/)

The goal of this project is to become obsolete and to get merged upstream.

Comment on this issue, if you'd like to see that happen: [Release binaries #6](https://github.com/awslabs/tc-redirect-tap/issues/6)

Want to download a binary? Head over to the releases page for Intel AMD and ARM64: [View releases](https://github.com/alexellis/tc-tap-redirect-builder/releases)

Since the upstream project has no tags, the release names use a date / time format i.e. : `2022-04-01-1328`

## Installation

```bash
mkdir -p /opt/cni/bin

export RELEASE=2022-04-01-1337

# For ARM64
export ARCH="-arm64"

# For AMD64
export ARCH=""

curl -SLs https://github.com/alexellis/tc-tap-redirect-builder/releases/download/$RELEASE/tc-redirect-tap$ARCH \
  -o  /opt/cni/bin/tc-redirect-tap
```

## License

Copyright 2022 Alex Ellis, OpenFaaS Ltd

License MIT
