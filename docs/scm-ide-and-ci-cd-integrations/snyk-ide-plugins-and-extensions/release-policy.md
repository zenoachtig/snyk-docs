# Release and Support policy for Snyk IDE plugins

This page details the release policy for Snyk IDE plugins.

Builds are deployed at distinct points in time after comprehensive testing and are considered stable.

**Cadence**: Six versions per year, approximately every **eight weeks**. Hotfix releases are possible for newly discovered security vulnerabilities.

## Versioning for IDE plugins

All Snyk IDE plugins follow industry standard [Semantic Versioning](https://semver.org/), which has a three-part notation. Given a version number, `MAJOR.MINOR.PATCH`, increment the:

1. `MAJOR` version when you make **breaking** changes; examples follow.
2. `MINOR` version when you add functionality in a backward-compatible manner.
3. `PATCH` version when you make backward-compatible bug fixes.

Release notes identify all changes, focusing on new features or significant changes.

Examples of **breaking** changes include the following:

* Deprecating features that produced findings before, which means users will get fewer findings after the release.
* Introducing new features that might introduce new findings.
* Introducing mandatory configuration changes that might affect the number of findings.

## Support policy

{% hint style="info" %}
This policy will be effective beginning on June 24, 2025.
{% endhint %}

Snyk supports the latest 12 months of plugin versions, ensuring functionality and performance. Older versions are considered End-of-Support (EOS) and will not receive bug fixes or troubleshooting.

Snyk only provides fixes in new versions and cannot fix older versions. Customers must upgrade to benefit from improvements.

This policy fosters innovation while optimizing resources.

If you need help, submit a [request](https://support.snyk.io) to Snyk Support.

## Preview builds

Snyk offers preview versions for those who want to test in-progress features.

{% hint style="info" %}
These versions may contain bugs and are not officially supported.
{% endhint %}

Preview builds are deployed regularly up to multiple times per day and contain the latest changes. They are given a version number following the pattern { YEAR }. { MONTH }.{ DAY }{ HOUR } .

Preview versions of IDE plugins are deployed as standalone plugins named in the form `(Preview) Snyk Security`. Snyk recommends that you not install them together with the stable version.
