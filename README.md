sgminer
sudo apt-get install build-essential libcurl4-openssl-dev git automake libtool libjansson* libncurses5-dev
git clone --recursive https://github.com/dmitriy79/gpu.git gpu
cd sgminer/
cp /opt/AMDADL/include/* ADL_SDK/
./autogen.sh
./configure CFLAGS="-O3 -Wall -march=native"
make
./sgminer -n
