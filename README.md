# PhantomJS 2.0 built on Ubuntu 14.04 x32

A clone from [the x64 version](https://github.com/Pyppe/phantomjs2.0-ubuntu14.04x64)
This repository contains a PhantomJS 2.0 -binary for Ubuntu. It was compiled on a Ubuntu 14.04.03 x32 non-virtual machine. See [PhantomJS #12948](https://github.com/ariya/phantomjs/issues/12948) for details.

### Download
```bash
wget https://github.com/fsoc/phantomjs2.0-ubuntu14.04x32/raw/master/bin/phantomjs
```

## What was done
```bash
sudo apt-get update
sudo apt-get install -y build-essential g++ flex bison gperf ruby perl libsqlite3-dev libfontconfig1-dev libicu-dev libfreetype6 libssl-dev libpng-dev libjpeg-dev

mkdir phantomjs
cd phantomjs
wget https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-2.0.0-source.zip
unzip phantomjs-2.0.0-source.zip

cd phantomjs-2.0.0/
time ./build.sh
```

#### Time to build
```
real    39m48.793s
user    122m25.136s
sys     8m49.940s
```

#### md5 / sha1
```
06865fe2838f5101b7a94aeca4d61b3b bin/phantomjs
dffbc2dd2665f18178623985c5d9b2a98eabc317  bin/phantomjs
```
