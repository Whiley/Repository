# Whiley Package Repository

This is the initial package repository for Whiley.  The intention is
that this is a temporary effort which will serve the community for a
short period.  A more complete solution will become available in the
near future.

## Usage

To use a package in Whiley (e.g. `std` version `0.2.15`, you must add
this to you `wy.toml` file:

```
[dependencies]
std="0.2.15"
html="0.1.7"
```

## Deployment

For now, to deploy a package into this repository you must make a pull
request against it.  Packages must be in the correct format, or the
request will be rejected automatically.  Specifically, the format is:

```
name/X.Y.Z/name-vX.Y.Z.zip
```

This is taken relative to the root of this repository.

## Other

To target a different package repository (such as your own GitHub
repository), you can override the default package URL by adding the
following to your `wy.toml` file:

```
[repository]
url="https://github.com/username/repo/raw/master"
```

This URL may contain additional information, such as the port number,
etc.