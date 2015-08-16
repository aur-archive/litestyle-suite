# Maintainer: jsteel <jsteel at aur.archlinux.org>

pkgname=litestyle-suite
_pkgname="Litestyle suite"
pkgver=0.2a
pkgrel=1
pkgdesc="Litestyle suite: BMPanel2, Conky, GTK+, Openbox, PekWM, Tint2, XFWM4 and Metacity themes"
arch=('any')
url="http://weakhead.deviantart.com/art/Litestyle-suite-148308075"
license=('GPL')
install=$pkgname.install
depends=('gtk-engine-murrine' 'ttf-droid')
source=(http://pkgbuild.com/~jsteel/aur/$pkgname/Litestyle_suite_by_weakhead.zip)
md5sums=('47ba5a2d859c48aa8cbc9cbcc2b1bc91')

# Shiki (bright colors) or Watered-down (fainter colors) for GTK
version=Watered-down

package() {
  install -dm755 "$pkgdir"/usr/share/themes
  cp -r "$srcdir"/"$_pkgname"/GTK\ and\ Openbox/$version\ range/* "$pkgdir"/usr/share/themes/
  cp -r "$srcdir"/"$_pkgname"/XFWM4\ and\ Metacity/Litestyle/ "$pkgdir"/usr/share/themes/

  install -dm755 "$pkgdir"/usr/share/pekwm/themes
  cp -r "$srcdir"/"$_pkgname"/PekWM/* "$pkgdir"/usr/share/pekwm/themes/

  install -dm755 "$pkgdir"/usr/share/bmpanel2/themes
  cp -r "$srcdir"/"$_pkgname"/BMPanel2/*/* "$pkgdir"/usr/share/bmpanel2/themes/

  install -dm755 "$pkgdir"/usr/share/$pkgname
  cp -r "$srcdir"/"$_pkgname"/{README,Conky,Tint2} "$pkgdir"/usr/share/$pkgname/
}
