sgminer
sudo apt-get install build-essential libcurl4-openssl-dev git automake libtool libjansson* libncurses5-dev
git clone --recursive https://github.com/dmitriy79/gpu.git gpu
cd sgminer/
cp /opt/AMDADL/include/* ADL_SDK/
./autogen.sh
./configure CFLAGS="-O3 -Wall -march=native"
make
./sgminer -n





git submodule init
git submodule update
autoreconf -i
CFLAGS="-O2 -Wall -march=native -std=gnu99" ./configure <options>
make
