
ACLOCAL_AMFLAGS = -I m4

bin_PROGRAMS = retry
retry_SOURCES = retry.c

EXTRA_DIST = retry.spec
dist_man_MANS = retry.1

dist-hook:
	which txt2man && ./retry --help | txt2man -d 1 -t "${PACKAGE_NAME}" -r "${PACKAGE_NAME}-${PACKAGE_VERSION}" > $(distdir)/retry.1 || true
