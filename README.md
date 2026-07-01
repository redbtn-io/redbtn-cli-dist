# redbtn CLI — keyless install

Public install tarballs for **`@redbtn/cli`** (the `redbtn` command-line connector).
No registry key required — install from a release asset; dependencies resolve from public npm.

## Install (latest)

```sh
npm i -g https://github.com/redbtn-io/redbtn-cli-dist/releases/download/v0.0.11-alpha/redbtn-cli-0.0.11-alpha.tgz
```

Then:

```sh
redbtn login          # OAuth device flow → app.redbtn.io
redbtn connect        # register this machine as an environment on your account
```

Optional native deps (skipped if unavailable): `keytar` (OS keychain), and
`@nut-tree-fork/nut-js` + `jimp` (desktop control via `redbtn connect --desktop-control`).

The authenticated package also lives at `registry.redbtn.io` as `@redbtn/cli`; this repo hosts the keyless tarballs.
