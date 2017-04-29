To compile for Debian

`apt-get install freebsd-glue libev-libevent-dev libevent-dev libutil-freebsd-dev qtcreator`

Then you'll have to make sure you add the include paths to `cc`'s include path.

```
C_INCLUDE_PATH=-I/usr/local/include
C_INCLUDE_PATH+=-I/usr/include
C_INCLUDE_PATH+=-I/usr/include/freebsd
C_INCLUDE_PATH+=-I/tmp/netmap/sys
C_INCLUDE_PATH+=-I/usr/lib/gcc/x86_64-linux-gnu/4.9/include
C_INCLUDE_PATH+=-I/usr/lib/gcc/x86_64-linux-gnu/4.9/include-fixed
C_INCLUDE_PATH+=-I/usr/include/x86_64-linux-gnu
CPATH=$C_INCLUDE_PATH
```
