# WOOWTECH KNXD add-on mirror

Mirror of the KNXD daemon add-on from [`da-anda/hass-io-addons`](https://github.com/da-anda/hass-io-addons) — the KNXD daemon lets you turn any Home Assistant OS box into a KNX/IP gateway via TPUART or USB bus adapters.

## Why this mirror

This mirror exists to guarantee availability if the upstream single-maintainer repo becomes unreachable. The `knxd/` add-on directory is a copy of the upstream tag `0.6.1`; the root `repository.yaml` retargets the repo for WOOWTECH-managed HAOS boxes.

## Upstream

- Source: https://github.com/da-anda/hass-io-addons/tree/main/knxd
- Version tracked: `0.6.1`
- Upstream maintainer: Franz Koch (`da-anda`)

## Usage

Two modes:

1. **HA store repo mode** — add this repo URL under Settings → Add-ons → three-dot menu → Repositories, then install "KNXD daemon" from the store.
2. **Local add-on mode** — copy the `knxd/` directory into `/addons/` on the HAOS box, `ha supervisor restart`, then install `local_knxd`.

For hardware wiring (TPUART / USB / IP), see the upstream `knxd/DOCS.md`.
