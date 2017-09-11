# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=obarun-zsh
pkgver=0.2
pkgrel=1
pkgdesc="obarun zsh setup"
arch=(x86_64)
url='https://obarun.org'
license=('BEERWARE')
depends=('zsh')
source=('zshrc' 'zshenv' 'LICENSE')
backup=('etc/skel/.zshrc' 'etc/skel/.zshenv' 'etc/.zshrc' 'etc/.zshenv')
sha256sums=('1aa7c5d56f9c3431601db21f24befcf0614751f0e3aedce4189d3f6363cf8fd8'
            'fdb6bb7bccd74fa09302276843b06d58073ca13593fa2ee4c93f59648dffa46c'
            '43cd6868c0ee7a193c72e08495c3beef9d8009b4e389e32c2ab71c9269a8e41a')
validpgpkeys=('6DD4217456569BA711566AC7F06E8FDE7B45DAAC') # Eric Vidal

package() {
	
	install -D -m644 zshrc ${pkgdir}/etc/skel/.zshrc
	install -D -m644 zshenv ${pkgdir}/etc/skel/.zshenv
	install -D -m644 zshrc ${pkgdir}/etc/.zshrc
	install -D -m644 zshenv ${pkgdir}/etc/.zshenv
	
	install -Dm 0644 "LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
