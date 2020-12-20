# Versioning policy and support

## Versioning

My projects aim to follow the [semantic versioning `^2`](https://semver.org/spec/v2.0.0.html).

Aside from few (documented) exceptions, if you install one of my
projects, you can expect that I will do my best to maintain its
API compatible with your project, at the major version you installed.

This means that, in an `X.Y.Z` versioning scheme:

 * `X` (major) means that something requires your action to upgrade
 * `Y` (minor) means that something has been added or improved, and you
   may benefit from it, if you put in the effort to get to that
   release.
 * `Z` (patch) means that something has been fixed: you should be able
   to upgrade without much thinking about it.

If you experience crashes or misbehavior when upgrading an `Y` or `Z`
version, you most probably encountered a bug that was not intended,
and should contact me through the affected project's issue tracker.

## Security

I take security very seriously, to the point that it will override most
rules/conventions defined in this article.

**DO NOT** report security issues on publicly accessible issue trackers:
by doing so, you effectively turn them into 0-day security issues. Be
responsible and consider that I do my work in good faith, when I have
time and will to do so.

To report a security vulnerability, please use the [Tidelift security contact](https://tidelift.com/security).
Tidelift will coordinate the fix and disclosure.

Alternatively, contact me at [ocramius+security@gmail.com](mailto:ocramius+security@gmail.com),
so that we can discuss a resolution.

## Backwards compatibility

I take backwards compatibility seriously, and I have written [tools](https://github.com/Roave/BackwardCompatibilityCheck)
and [spoken at conferences](https://vimeo.com/345919162) about it.

If you find a backwards-incompatible change in a minor version of my library,
please do open an issue on the associated project.

## Dependency upgrades

I regularly upgrade dependencies and dependency requirements for my
projects, and often do have automation in place to do so at set time
intervals.

Dependency changes will **only** take place in `X` (major) and `Y`
(minor) releases,  and will not be performed for `Z` (patch) releases,
unless a security issue overrules this.

Every new `X` or `Y` version I release can be expected to restrict
dependency requirements to the latest and greatest of these dependencies,
unless the API signature of my project would also change in doing so.

This is done consciously/intentionally: in practice, if you want the
latest features from one of my projects, you must put in the effort to
meet mid-way and upgrade your other dependencies too.

If you cannot upgrade because of external constraints in your environment
(human or technological) prevent you to do so, then there is probably
an older version of my library that still runs on your system: try relaxing
your dependency constraints.

In addition to the above rationale, and in concordance with
["Why I do open source"](./why-i-do-open-source.md), I upgrade dependencies
also because I do keep myself updated and educated about what other tools
provide as "latest and greatest", and I quickly move on.

Please note that [dependency upgrades are also semver-compliant](https://semver.org/spec/v2.0.0.html#what-should-i-do-if-i-update-my-own-dependencies-without-changing-the-public-api).

## Support policy

What you can expect me to do is to release bugfixes in versions of my packages
that are in their "latest and greatest" release: means that generic bugs
will be fixed in the last `X.Y` release.

Should a bug be of critical, security or "game breaking" relevance,
then I will attempt to apply such a fix to all versions that are compatible
with the ecosystem's "supported versions".

This means that  I will look for [EOL](https://en.wikipedia.org/wiki/End-of-life_product)'d
dependencies and categorically exclude fixing bugs (and accepting patches)
for such outdated releases: you had time to upgrade, and if the update is
not possible, you need to make this a critical priority in your environment.

All versions that support contemporary dependencies will receive critical
and security bugfixes, until one or more of the supported dependencies
reaches [EOL](https://en.wikipedia.org/wiki/End-of-life_product).

### When will my bug be fixed?

I do not actively provide support for my work: it is all done in good
faith, within the time constraints of "after work", "in the weekend",
and most importantly **when I want to do it**.

I'll fix bugs on my end, but remember that this happens in conflict with
other interests that you may be unaware of.

## "Forcing" support

Despite that, you can bribe me into offering you paid support through
a consultancy contract ([contact me](mailto:ocramius@gmail.com)), or
by sponsoring me substantially on [github sponsors](https://github.com/sponsors/Ocramius).

In addition to that, [Tidelift](https://tidelift.com/) subscribers do
get Tidelift to chase me down if I did something wrong: I am a responsible
human being, so I don't expect things to go wrong under my watch, but
things can and will always go wrong, according to [Murphy's law](https://en.wikipedia.org/wiki/Murphy%27s_law).

Yes, by forcing the hand you are becoming a paying customer, and get
to have a say in how things are done, but like with every business
relationship, discussions must be taken.
