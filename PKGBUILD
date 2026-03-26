# Maintainer: vbopk9x3 <vbopk9x3@4wrd.cc>
pkgname=pangolin-bin
pkgver=0.5.3
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
sha256sums_x86_64=('6d952e715f36a7222e1265b15c21fd0ef5ac75bc3f9e3ed1fe18f5bc0980fff8')
sha256sums_aarch64=('a3902ac3023b13761d66ff3757873b6912dc680ba07c2a231ce50f4110c994f4')
sha256sums_armv7h=('61ee0369613393e55537b3cedd87ed11e3f1d473163dc731935ab332252caefd')
sha256sums_armv6h=('1f57052bfcfe72827b60303353ef08fa6099e2338d9aa4839bd3451aabf06328')
sha256sums_riscv64=('2340b5afd8f3bb9b57679f43e044421b6aea0fc4554c4d77503308bdd52d7c37')

package() {
    # Install the binary to /usr/bin and set executable permissions
    install -Dm755 "${srcdir}/pangolin" "${pkgdir}/usr/bin/pangolin"
}
