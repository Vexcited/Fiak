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
quilt pop -af

# update upstream to a given version
cd yaak
git fetch --tags
git checkout v2025.9.3 # for example
cd ..

# commit the new pointer
git add yaak
git commit -m 'chore(yaak): upgrade to v2025.9.3'

# apply all patches
quilt push -af
```

Pray there's no conflict, if that's the case,
resolve them through `refresh` and `push`.
