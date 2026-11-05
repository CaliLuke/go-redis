# Temporary root-module publication

This root module follows upstream `redis/go-redis` master at
`5cba5e18` with only root-module and self-import paths renamed to
`github.com/CaliLuke/go-redis/v9`. The full upstream source identity is the
parent commit of this module-publication commit.

Upstream [PR #4095](https://github.com/redis/go-redis/pull/4095) preserves hooks
when cloning a client with `WithTimeout`. It has merged into master but is not
in the latest stable release, v9.23.0. No duplicate patch is applied here.
Return to a stable upstream release once it contains the correction and passes
the hook-preservation and shutdown regressions.

Nested extension, example and tooling modules retain their upstream identities;
they are not published as fork modules. Types from those upstream modules are
not interchangeable with this root module's types.
