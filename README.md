<div align="center">

# pushinbr/pam-core-api

## Compatibility package — do not use in new applications

This repository exists so older Composer projects keep installing safely. The maintained product is **[PAM Contracts](https://github.com/push-in/pam-contracts)**.

[![Replacement](https://img.shields.io/badge/replacement-pushinbr/pam--contracts-2563eb?style=flat-square)](https://packagist.org/packages/pushinbr/pam-contracts)
![Status](https://img.shields.io/badge/status-migration%20only-f59e0b?style=flat-square)

</div>

---

## Use this instead

```bash
pam composer require pushinbr/pam-contracts
```

[PAM Contracts](https://github.com/push-in/pam-contracts) contains the active documentation, API examples, releases, issue tracker, and production guidance.

## Why the name changed

The replacement describes the package accurately: stable extension contracts, not an API framework or runtime core.

## Migrate an existing project

Commit your current `composer.json` and `composer.lock`, then run:

```bash
pam composer remove pushinbr/pam-core-api
pam composer require pushinbr/pam-contracts
pam doctor
```

Run the application test suite before committing the new lockfile. Composer may continue to resolve this bridge transitively during a staged migration; application code should target the replacement package directly.

## Support policy

- No new features are added here.
- Security or resolution fixes may be published only to preserve migration safety.
- New documentation and issues belong to [PAM Contracts](https://github.com/push-in/pam-contracts).
- The package is marked abandoned on Packagist in favor of `pushinbr/pam-contracts`.

This explicit compatibility repository is intentional: old installs remain understandable without making the current PAM ecosystem ambiguous.
