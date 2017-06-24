### kubler/pure-ftpd:20170521

Built: Sun May 21 22:05:59 CEST 2017
Image Size: 18.7 MB

#### Installed
Package | USE Flags
--------|----------
dev-libs/libsodium-1.0.11 | `asm urandom -minimal -static-libs`
net-ftp/ftpbase-0.01-r2 | `-pam`
net-ftp/pure-ftpd-1.0.45-r1 | `ssl vchroot -anondel -anonperm -anonren -anonres -caps -charconv -implicittls -ldap (-libressl) -mysql -noiplog -pam -paranoidmsg -postgres -resolveids (-selinux) -sysquota -xinetd`
*manual install*: syslog-stdout-1.1.1 | https://github.com/timonier/syslog-stdout
#### Inherited
Package | USE Flags
--------|----------
**FROM kubler/openssl** |
app-misc/ca-certificates-20161102.3.27.2-r2 | `-cacert -insecure`
app-misc/c_rehash-1.7-r1 | ``
dev-libs/openssl-1.0.2k | `asm sslv3 tls-heartbeat zlib -bindist -gmp -kerberos -rfc3779 -sctp -sslv2 -static-libs {-test} -vanilla`
sys-apps/debianutils-4.7 | `-static`
sys-libs/zlib-1.2.11 | `-minizip -static-libs`
**FROM kubler/s6** |
dev-lang/execline-2.3.0.0 | `-static -static-libs`
dev-libs/skalibs-2.5.0.0 | `-doc -ipv6 -static-libs`
sys-apps/s6-2.5.0.0 | `-static -static-libs`
*manual install*: entr-3.6 | http://entrproject.org/
**FROM kubler/glibc** |
sys-apps/gentoo-functions-0.10 | ``
sys-libs/glibc-2.23-r3 | `hardened rpc -audit -caps -debug -gd (-multilib) -nscd (-profile) (-selinux) -suid -systemtap -vanilla`
sys-libs/timezone-data-2017a | `nls -leaps`
**FROM kubler/busybox** |
sys-apps/busybox-1.25.1 | `make-symlinks static -debug -ipv6 -livecd -math -mdev -pam -savedconfig (-selinux) -sep-usr -syslog -systemd`
#### Purged
- [x] Headers
- [x] Static Libs