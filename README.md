# linux-cachyos-bore

## I cannot guarantee reliability and that it will build on every machine, it works fine on my NVIDIA desktop

CachyOS kernel with BORE scheduler packaged for Void Linux (via xbps-src).

If kernel headers are wanted an symlink must be created
```
ln -s srcpkgs/linux-cachyos-bore srcpkgs/linux-cachyos-bore-headers
```

Copy the `srcpkgs/linux-cachyos-bore/` directory into a `void-packages` checkout and build:

```
./xbps-src pkg linux-cachyos-bore
```

Install:

```
sudo xbps-install -R hostdir/binpkgs linux-cachyos-bore linux-cachyos-bore-headers
```
