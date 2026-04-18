# Maintainer: vbopk9x3 <vbopk9x3@4wrd.cc>
pkgname=pangolin-bin
pkgver=0.6.0
pkgrel=1
pkgdesc="Pangolin Client - Secure reverse proxy and tunnel (Binary version)"
arch=('x86_64' 'aarch64' 'armv7h' 'armv6h' 'riscv64')
url="https://github.com/fosrl/cli"
license=('AGPL-3.0-or-later')
provides=('pangolin')
conflicts=('pangolin')
install=pangolin-bin.install

source_x86_64=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_amd64")
source_aarch64=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_arm64")
source_armv7h=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_arm32")
source_armv6h=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_arm32v6")
source_riscv64=("pangolin::https://github.com/fosrl/cli/releases/download/${pkgver}/pangolin-cli_linux_riscv64")

# SHA256 Checksums (Generate these using 'updpkgsums')
sha256sums_x86_64=('2e2e1f78ed8517633e6e05823e2e2808b3d8d8730005797732777b0f3e27c7ec')
sha256sums_aarch64=('74e24dff95a86bead5731fa51c2d018a29d6db602847b3e8fdc9fc8dd02c1408')
sha256sums_armv7h=('8c02292aeac56ba192556118f5a564935a16dc2fddbfd5869ac41427b69fc60a')
sha256sums_armv6h=('c077c28bf0f40c5ae160d7718ec0379a5c794429d816b3bc928eff0e6a6fc082')
sha256sums_riscv64=('edd6423e5556e70a51037aa75b4a6cacc1b9043e3c4a87ebfb42a4161769b505')

package() {
    # Install the binary to /usr/bin and set executable permissions
    install -Dm755 "${srcdir}/pangolin" "${pkgdir}/usr/bin/pangolin"
}
