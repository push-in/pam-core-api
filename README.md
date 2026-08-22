# pushinbr/pam-core-api

This name is retained only for migration compatibility. The package is now
[`pushinbr/pam-contracts`](https://packagist.org/packages/pushinbr/pam-contracts).

## Start here

```bash
curl -fsSL https://push-in.github.io/pam/install.sh | sh
pam doctor
pam composer remove pushinbr/pam-core-api
pam composer require pushinbr/pam-contracts
```

Existing projects may keep resolving this package temporarily because it
depends on the replacement. New code must require `pushinbr/pam-contracts` directly.
