# Maintainer: Senventise <senventise@gmail.com>

pkgname=video-compress-context
pkgver=0.3
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
  "6d3783bb5979d44b820289b45bab8dc44e66eae36e1a022e1aa4ce154d41f799"
  "a71e5c114fcbdfba6a0f1e87a36e160d7fe8579e155c084bb8799fc9980c6386"
)

package() {
  install -Dm755 com.senventise.vcompress.desktop -t "${pkgdir}/usr/share/kio/servicemenus/"
  install -Dm755 vcompress_gui -t "${pkgdir}/usr/bin/"
}
