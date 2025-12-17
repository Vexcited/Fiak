# Fiak

A release build of [Yaak](https://github.com/mountain-loop/yaak) without the `license` code.

## Motivation

Yes, I know Yaak is forever free and will never force you to pay a license in any way.

However I don't like seeing `Commercial Trial` or a `Purchase License` button in menus.
Most people will go along and not care that much but that kinda ruins the beauty of the product to me.

Thankfully, all the licensing code is behind a `license` feature (enabled by default in release configuration) so if we don't want all of this, we can just build a release without that feature.

I also wanted to learn how managing a patchset is done at the same time.

## Included

- Remove that one useless mention about telemetry
- Rebranding to `Fiak` instead of `Yaak`
- Build without the `license` feature

Concerning releases, Fiak is updated whenever Yaak create a new release.

## Develop

Take a look at [CONTRIBUTING](./CONTRIBUTING.md) to know how to setup the repository.
