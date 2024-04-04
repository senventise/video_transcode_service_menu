# Maintainer: Senventise <senventise@gmail.com>

pkgname=video-compress-context
pkgver=0.4
pkgrel=1
pkgdesc="Convert video into hevc with context menu."
arch=("x86_64")
url="https://github.com/senventise/video_transcode_service_menu"
license=('MIT')

depends=(
  "mediainfo"
  "ffmpeg"
  "trash-cli"
  "kdialog"
)

source=(
  "vcompress_gui"
  "com.senventise.vcompress.desktop"
)

sha256sums=(
  "4fe1876cbcbf79954d7b47037e1015a2878809383779207ccd5e35a9b03d18d3"
  "a71e5c114fcbdfba6a0f1e87a36e160d7fe8579e155c084bb8799fc9980c6386"
)

package() {
  install -Dm755 com.senventise.vcompress.desktop -t "${pkgdir}/usr/share/kio/servicemenus/"
  install -Dm755 vcompress_gui -t "${pkgdir}/usr/bin/"
}
