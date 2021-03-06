emqx-packages
=============

EMQ X RPM/Debian Packages

NOTICE: Requires Erlang/OTP R21+ to build since 3.0 release.

Build on Linux Debian/Ubuntu
----------------------------

```
make
sudo dpkg -i emqx-${PKG_VSN}-amd64.deb
```

Build on Linux Centos/Redhat
----------------------------

```
yum install rpm-build
make
sudo rpm -ivh emqx-${PKG_VSN}-1.el7.x86_64.rpm
```

Build version other than default defined in Makefile
----------------------------------------------------

```
export PKG_VSN=<version>
export REL_TAG=<tag-or-branch>
export EMQX_DEPS_DEFAULT_VSN=<tag-or-branch>
make
```

License
-------

Apache License Version 2.0

Author
------

EMQ X Team.
