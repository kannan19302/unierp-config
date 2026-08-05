# unierp-config

**Layer L1 — Foundation** of the [UniERP](../unierp-platform) platform.
Depends on: nothing.

## What this is

Shared TypeScript and Prettier configuration.

## The invariant this repository owns

Every repo extends this rather than copying it. A hand-copied config is how the Dockerfile bug of § 1.1 propagated to four repositories and was fixed three separate times.

## The rule that applies everywhere

A repository may depend only on published artifacts of a **strictly lower
layer** — never sideways within a layer, never upward. A cycle is not
discouraged; it is unrepresentable, because the lower layer's package cannot
name the higher one.

See the [platform overview](../unierp-platform/README.md) for the full map, and
[`PLATFORM_ARCHITECTURE.md`](../ERPSys/docs/PLATFORM_ARCHITECTURE.md) § 4.2 for
the reasoning.

## Licence

AGPL-3.0.
