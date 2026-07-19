# hablab-updates

The public update channel ("shelf") for the **HAB•LAB** WordPress plugin
(slug `hablab`) — served by GitHub Pages at
`https://blazzzar.github.io/hablab-updates/`.

Sites running HAB•LAB read `hablab.json` (which versions exist on
the `stable` and `beta` tracks, plus retained releases for one-click
rollback) and download the built zips from `zips/`.

Nothing sensitive lives here: the zips contain only the plugin code — no
tracker data, no passphrase, no keys. The source, history, and docs live
in the private [`hablab`](https://github.com/Blazzzar/hablab)
repo.

**Don't edit this repo by hand** — `bin/publish-channel.sh` in the code
repo writes the manifest, adds the new zip, trims retention to the last
5 releases, and prunes unreferenced zips.
