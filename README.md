## Btree, ported to ZeroVM

----

To compile:

0. Working [toolchain][gcc] is needed.
1. Build and install [zlib port][zlib] and [openssl port][ssl].
2. Compile the test executable:

~~~~
git clone https://github.com/zerovm/ztree
cd ztree
x86_64-nacl-gcc -DDEBUG -g -o btest.nexe src/btest.c src/btree.c -Icompat -lcrypto
~~~~

[gcc]: https://github.com/zerovm/toolchain
[zlib]: https://github.com/zerovm/zerovm-ports/tree/master/zlib
[ssl]: https://github.com/zerovm/zerovm-ports/tree/master/openssl

