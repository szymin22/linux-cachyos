# linux-cachyos-void
## CachyOS Kernel with BORE built for void linux using xbps-src with pre-built packages in releases.
Based on the linux7.1 xbps-src packages, changes were made by OpenCode

## I cannot guarantee reliability and that it will build on every machine, it works fine on my NVIDIA desktop

If kernel headers are wanted an symlink must be created (especially when using nvidia or other DKMS modules)
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
