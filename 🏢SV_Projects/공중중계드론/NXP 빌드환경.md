Ubuntu 24.04 기준

툴체인 설치
```
wget https://snapshots.linaro.org/gnu-toolchain/12.1-2022.08-1/aarch64-linux-gnu/gcc-linaro-12.1.1-2022.08-x86_64_aarch64-linux-gnu.tar.xz

sudo mkdir -p /opt
cd /opt
sudo tar -xf ~/gcc-linaro-12.1.1-2022.08-x86_64_aarch64-linux-gnu.tar.xz

ls /opt/gcc-linaro-12.1.1-2022.08-x86_64_aarch64-linux-gnu.tar.xz

echo 'export PATH=/opt/gcc-linaro-12.1.1-2022.08-x86_64_aarch64-linux-gnu/bin:$PATH' >> ~/.bashrc
source ~/.bashrc

aarch64-linux-gnu-g++ --version
```

컴파일
```
aarch64-linux-gnu-g++ gpio_mult.c -o gpio_mult
```