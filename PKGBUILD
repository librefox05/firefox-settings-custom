_name=firefox-settings-custom
_channel=stable
_lang=en-US
_pkgname="${_name}"
pkgname="firefox-settings-custom"
provides=('firefox-settings-custom')
conflicts=('firefox-settings-custom')
pkgdesc="Custom firefox settings for a privacy first firefox experience(${_lang})"
pkgver=145.0
pkgrel=1
tag=${pkgver}-1
arch=('x86_64' 'aarch64')
license=('MPL' 'GPL' 'LGPL')

depends=(
  'firefox'
)

source=(
  "librefox.cfg"
  "autoconfig.js"
)

sha256sums=(
  'SKIP'
  'SKIP'
)

package() {
  FF_PATH="usr/lib/firefox"
  FF_DEF_PATH="${FF_PATH}/defaults/pref"

  # Install the package files
  install -d "${pkgdir}"/"${FF_PATH}"
  mkdir -p ${pkgdir}/${FF_DEF_PATH}
  cp autoconfig.js ${pkgdir}/"${FF_DEF_PATH}"
  cp librefox.cfg ${pkgdir}/${FF_PATH}

}
