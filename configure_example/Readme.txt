Ref:
	https://www.idryman.org/blog/2016/03/10/autoconf-tutorial-1/

how to compile:
**************
autoreconf --force --install --verbose
./configure 
make
make install DESTDIR="${PWD}/gar"

Note: make install will install bins in host pc so give other path




CROSS COMPILE for ARM:
**********************
add your toolchain to configure file 
	./configure --host=arm-linux-gnueabi


e.g:

autoreconf --force --install --verbose
./configure --host=arm-linux-gnueabi
make
make install DESTDIR="${PWD}/gar"




