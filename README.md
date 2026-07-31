# node-tiddlywiki-debian

[![Debian Build Bot](https://github.com/donmor/node-tiddlywiki-debian/actions/workflows/packaging.yml/badge.svg)](https://github.com/donmor/node-tiddlywiki-debian/actions/workflows/packaging.yml)

(Unofficial) Debian packaging scripts for [tiddlywiki](https://www.npmjs.com/package/tiddlywiki).

Provided packages:
- `node-tiddlywiki`

## Quick configuration
Install [`donmor-repos-keyring`](https://donmor-repos.github.io/pub/donmor-repos-keyring_0.0.1_all.deb) and [`node-tiddlywiki-debian-repo`](https://donmor-repos.github.io/pub/node-tiddlywiki-debian-repo_0.0.1_all.deb), then run `apt-get update`.
 
## Manual configuration
#### Add keyring:
``` bash
curl -sLOJR --output-dir /usr/share/keyrings https://donmor-repos.github.io/pub/donmor-repos-keyring.gpg
```
#### Add `node-tiddlywiki-debian`:
``` bash
tee /etc/apt/sources.list.d/node-tiddlywiki.sources <<EOF
Types: deb deb-src
URIs: https://github.com/donmor/node-tiddlywiki-debian/releases/latest/download
Suites: /
Signed-By: /usr/share/keyrings/donmor-repos-keyring.gpg
EOF
apt-get update
```
