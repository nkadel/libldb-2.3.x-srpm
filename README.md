libldb-2.1.x-srpm
=================

SRPM building tools for libldb-2.1.x for runing Samba 4 on RHEL and Fedora
=======

Required rebuild with libtdb updates for Samba.

These are built from Fedora rawhide releases, and need to be built and
installed in the following order.

	libtalloc-2.3.x-srpm
	libtdb-1.4.x-srpm
	libldb-2.1.x-srpm
	libtevent-0.10.x-srpm

	samba-4.11.x-srpm

The "make" command will do these steps.

	make build	# Build the package on the local OS
	make all	# Use "mock" to build the packages with the local
			# samba4repo-6-x96_64 configuration, which needs.
	make install	# Actually install the RPM's in the designated
			# location for samba4repo-6-x86_64


		Nico Kadel-Garcia <nkadel@gmail.com>
