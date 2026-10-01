# redbtn CLI — keyless install

Public install tarballs for **`@redbtn/cli`** (the `redbtn` command-line connector).
No registry key required — install from a release asset; dependencies resolve from public npm.

> **This install path is retired.** Get the CLI (and redbtn Desktop) from the
> download page: **https://redbtn.io/download**
>
> ```sh
> curl -fsSL https://redbtn.io/install.sh | sh
> ```
>
> Already installed? Update any time with `redbtn update`. The tarballs below
> stay for history; new releases ship on the public channel instead.

## Install (latest)

```sh
curl -fsSL https://redbtn.io/install.sh | sh
```

Then:

```sh
redbtn login          # OAuth device flow → app.redbtn.io
redbtn connect        # register this machine as an environment on your account
```

Optional native deps (skipped if unavailable): `keytar` (OS keychain), and
`@nut-tree-fork/nut-js` + `jimp` (computer-use via `redbtn connect --see --control`).

The authenticated package also lives at `registry.redbtn.io` as `@redbtn/cli`; this repo hosts the keyless tarballs.
