# Maintainer Matz Radloff <matzradloff@gmail.com>
# Developer kishorv06 <https://github.com/kishorv06>

pkgname=mkinitcpio-clevis-hook-curl
pkgver=1.0
pkgrel=1
pkgdesc="A simple hook to unlock LUKS devices on boot with clevis and TPM or Tang on Arch Linux and its derivatives, including the non-systemd versions"
arch=('any')
url="https://github.com/timesqueezer/arch-mkinitcpio-clevis-hook"
license=("GPL3")
depends=("clevis" "tpm2-tools" "luksmeta" "libpwquality" "mkinitcpio" "tpm2-abrmd" "curl")
makedepends=("git")
conflicts=("mkinitcpio-clevis-hook")
source=("git+$url.git/")
md5sums=("SKIP")
build() {
  printf ""
}
package() {
  mkdir -p "$pkgdir"/etc/initcpio/hooks/
  mkdir -p "$pkgdir"/etc/initcpio/install/
  install -Dm644 "$srcdir"/arch-mkinitcpio-clevis-hook/hooks/clevis "$pkgdir"/etc/initcpio/hooks/
  install -Dm644 "$srcdir"/arch-mkinitcpio-clevis-hook/install/clevis "$pkgdir"/etc/initcpio/install/
}
