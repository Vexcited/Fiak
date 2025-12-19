# Fiak

A release build of [Yaak](https://github.com/mountain-loop/yaak) without the `license` code - and a few more things.

## Why ?

I know Yaak is free and always will be, there’s no requirement to buy a license.

That said, I’m not a fan of seeing things like `Commercial Trial` or `Purchase License` in the UI. Most people probably don’t care, but for me it slightly takes away from how nice the app feels.

Luckily, all the licensing stuff is behind a `license` feature flag, enabled by default in release builds. If you build without it, all of that simply disappears.

I also used this project as an excuse to learn how patchsets work and how to maintain one properly.

And finally, as a French person, naming a Yaak alternative Fiak was too perfect to pass up.

## Included

- Remove that one useless mention about telemetry
- Rebranding to `Fiak` instead of `Yaak`
- Build without the `license` feature

## Versions

Fiak is updated whenever Yaak creates a new release.
This a manually done process. Please open an issue if I'm too slow to update Fiak.

Fiak adds an additional number to the version which is the release count for this specific Yaak version.

> For example, `v2025.9.3` will have its first Fiak version as `v2025.9.3.0`. If Fiak applies a new patch and release, it'll be `v2025.9.3.1`.

## What did not change internally ?

- `User-Agent` for the internal API since the plugin store requires the Yaak one to prevent us getting an Internal Server Error
- `yaak` deep link scheme to keep Fiak compatible with Yaak integrations

## Let's work together !

Take a look at [CONTRIBUTING](./CONTRIBUTING.md) to know how to setup the repository.
