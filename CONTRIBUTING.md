# Contributing

You must have [`quilt`](https://savannah.nongnu.org/projects/quilt) to work with patches.

## Quick Start

```sh
# clone fiak with yaak submodule
git clone --recurse-submodules https://github.com/Vexcited/Fiak

# apply all patches
quilt push -a
```

Follow instructions in [`yaak/DEVELOPMENT.md`](./yaak/DEVELOPMENT.md) if you
want to build Fiak locally.

## Updating upstream

```sh
# remove all patches
quilt pop -a

# update upstream
git submodule update --remote yaak

# apply all patches
quilt push -a
```

Pray there's no conflict, if that's the case,
resolve them through `refresh` and `push`.
