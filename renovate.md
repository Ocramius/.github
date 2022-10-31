# Renovate integration

Repositories under the [`ocramius/`](https://github.com/Ocramius/) scope receive regular dependency
upgrades through [renovate](https://github.com/renovatebot/renovate/tree/f50e685fe425ce9c4dfcf439d6edacb4906c49e3),
which automates the heavy lifting of uplading lock files, supported dependency ranges, etc.

This is defined in [`renovate-config.json`](./renovate-config.json), and imported in all applicable
repositories in the organization.

Dependency ranges are kept restrictively recent as per my [version support](./version-support.md) policy.

The configuration is heavily inspired by the
[`laminas/.github` one](https://github.com/laminas/.github/blob/cbcde244afaa457a5a8fae957581ed9abf2a50da/renovate-config.json).

To use this configuration, create a [`renovate.json`](./renovate.json) file in the repository where it should be active:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "local>ocramius/.github:renovate-config"
  ]
}
```

Please note that this file will change according to **MY OWN** needs: no BC guaranteed. I endorse that
you copy the configuration and adapt it yourself, should you need it.
