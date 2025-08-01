### sudo apt install build-essential libtool autotools-dev automake pkg-config bsdmainutils curl git nsis g++-mingw-w64-x86-64
### git clone https://github.com/bitcoin/bitcoin.git
### cd bitcoin/depends
### sudo update-alternatives --config x86_64-w64-mingw32-g++ # Здесь нужно нажать цифру соответствующую строке "/usr/bin/x86_64-w64-mingw32-g++-posix" и enter
### PATH=$(echo "$PATH" | sed -e 's/:\/mnt.*//g')
### make HOST=x86_64-w64-mingw32
### cd ..
### ./autogen.sh
### CONFIG_SITE=$PWD/depends/x86_64-w64-mingw32/share/config.site ./configure --prefix=/
### make
### make install DESTDIR=/mnt/c/workspace/bitcoin


