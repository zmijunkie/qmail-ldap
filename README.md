# qmail-ldap
qmail-ldap port for FreeBSD12 goes OPENSSL_VERSION_NUMBER >= 0x10100000L, my own version - work in progress

Just want to use this software for OPENSSL_VERSION_NUMBER >= 0x10100000L

This it was I do to compile mal qmail-ldap:


portsnap fetch update
cd /usr/ports/mail
rm -rf qmail-ldap/
git clone https://github.com/zmijunkie/qmail-ldap
./install_new_patch
make extract
make patch
make
make install

Try this on your own risk. Works for me.
