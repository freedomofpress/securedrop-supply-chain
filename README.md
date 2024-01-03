# SecureDrop's Rust crate audits

SecureDrop uses [cargo-vet](https://mozilla.github.io/cargo-vet/index.html)
to ensure third-party Rust dependencies have been audited  by us or another trusted entity (e.g. [Mozilla](https://github.com/mozilla/supply-chain));
see [our documentation](https://developers.securedrop.org/en/latest/dependency_updates.html#auditing-rust-dependencies)
for more details.

This repository automatically [aggregates](https://mozilla.github.io/cargo-vet/multiple-repositories.html)
our audits from various repositories to make them easily reusable by others.

To import our audits into another cargo-vet instance, add the following
lines to your config.toml:
```toml
[imports.securedrop]
url = "https://raw.githubusercontent.com/freedomofpress/securedrop-supply-chain/main/audits.toml"
```
