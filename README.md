# renovate-rustls-repro

Minimal reproduction for a Renovate changelog issue: the `rustls` crate is
pinned to `=0.23.43`. Renovate proposes an update to `0.23.45`, but the PR
body contains no release notes and no compare URL, because rustls tags its
GitHub Releases as `v/0.23.45` (with a `v/` prefix), which Renovate's
changelog tag matching cannot reduce to the version `0.23.45`.

See: https://github.com/rustls/rustls/tags
