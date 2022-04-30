dist_bin_SCRIPTS =
dist_bin_SCRIPTS += extractenator

dist_sysconf_DATA =
dist_sysconf_DATA += extractenator.conf

pkgdata_DATA =
pkgdata_DATA += extractenator.sh


install-exec-hook:
	sed -i 's|__LIBDIR__|$(pkgdatadir)|' $(DESTDIR)$(bindir)/extractenator
	sed -i 's|__CONFDIR__|$(sysconfdir)|' $(DESTDIR)$(bindir)/extractenator
