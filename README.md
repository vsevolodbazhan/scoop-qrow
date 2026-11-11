# Qrow Scoop bucket

[![Tests](https://github.com/vsevolodbazhan/scoop-qrow/actions/workflows/ci.yml/badge.svg)](https://github.com/vsevolodbazhan/scoop-qrow/actions/workflows/ci.yml) [![Excavator](https://github.com/vsevolodbazhan/scoop-qrow/actions/workflows/excavator.yml/badge.svg)](https://github.com/vsevolodbazhan/scoop-qrow/actions/workflows/excavator.yml)

[Scoop](https://scoop.sh) manifests for [Qrow](https://github.com/vsevolodbazhan/qrow),
a desktop SQL workbench.

## Install

```pwsh
scoop bucket add qrow https://github.com/vsevolodbazhan/scoop-qrow
scoop install qrow
```

To install the latest nightly build, use `scoop install qrow-nightly`. You can
install the two packages at the same time. They use the same workspace and
settings.

To upgrade, use `scoop update qrow` or `scoop update qrow-nightly`. Close Qrow
before you upgrade it.

## Packages

| Package | Release |
| --- | --- |
| `qrow` | The latest stable release |
| `qrow-nightly` | The latest nightly prerelease |

Both packages install the portable Windows archive of the release for x86-64
or ARM64. The archive is not signed.

## Updates

The [Excavator workflow](.github/workflows/excavator.yml) runs every hour. It
finds new Qrow releases on GitHub, downloads the archives, calculates their
SHA-256 checksums, and commits the updated manifests. Do not edit the version,
URLs, or hashes manually.

Report problems with Qrow in the
[Qrow repository](https://github.com/vsevolodbazhan/qrow/issues).
