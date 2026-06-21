# linux-cachyos-bore

CachyOS kernel with BORE scheduler packaged for Void Linux (via xbps-src).

Copy the `srcpkgs/linux-cachyos-bore/` directory into a `void-packages` checkout and build:

```
./xbps-src pkg linux-cachyos-bore
```

Install:

```
sudo xbps-install -R hostdir/binpkgs linux-cachyos-bore linux-cachyos-bore-headers
```
