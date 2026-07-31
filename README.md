# node-tiddlywiki-debian

[![Debian Build Bot](https://github.com/donmor/node-tiddlywiki-debian/actions/workflows/packaging.yml/badge.svg)](https://github.com/donmor/node-tiddlywiki-debian/actions/workflows/packaging.yml)

(Unofficial) Debian packaging scripts for [tiddlywiki](https://www.npmjs.com/package/tiddlywiki).

``` bash
# tee /etc/apt/sources.list.d/node-tiddlywiki.list <<EOF
deb [trusted=yes] https://github.com/donmor/node-tiddlywiki-debian/releases/latest/download /
# deb-src [trusted=yes] https://github.com/donmor/node-tiddlywiki-debian/releases/latest/download /
EOF
```
