# sgminer
sudo apt-get install build-essential libcurl4-openssl-dev git automake libtool libjansson* libncurses5-dev
**releases**: git clone --recursive https://github.com/dmitriy79/gpu.git gpu
**releases**: cd sgminer/
**releases**: cp /opt/AMDADL/include/* ADL_SDK/
**releases**: ./autogen.sh
**releases**: ./configure CFLAGS="-O3 -Wall -march=native"
**releases**: make
**releases**: ./sgminer -n
