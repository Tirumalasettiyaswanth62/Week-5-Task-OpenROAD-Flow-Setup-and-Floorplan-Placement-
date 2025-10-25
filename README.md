# Week-5-Task-OpenROAD-Flow-Setup-and-Floorplan-Placement-
VSD RISC-V TAPEOUT PROGRAM WEEK-5 ASSIGNMENT 

## Steps to install OpenROAD :

#### Clone the git : 
``` 
git clone --recursive https://github.com/The-OpenROAD-Project/OpenROAD.git 
```
### Follow these steps :

#### step1:
```
1.git clone https://github.com/google/or-tools.git

2.cd or-tools

3.mkdir build && cd build
cmake -DBUILD_DEPS=ON -DCMAKE_BUILD_TYPE=Release ..

4.make -j$(nproc)

5.sudo make install
```

#### step2:
```
1.git clone this one https://github.com/The-OpenROAD-Project/OpenROAD.git

2.cd OpenROAD/

3.rm -rf build

4.mkdir build

5.cd build
```

#### step3:
```
1.cd third-party

2.git clone https://github.com/gabime/spdlog.git
cd ..
```

#### step4:
```
1.sudo add-apt-repository

2.ppa:ubuntu-toolchain-r/test -y

3.sudo apt update

4.sudo apt install g++-9 -y
```

#### step5:
```
cmake .. -DCMAKE_BUILD_TYPE=Release
#### if you occur any error ... follow the below commands
-DCMAKE_CXX_FLAGS="-Wno-error"

-DCMAKE_PREFIX_PATH="/usr/local"

-DCMAKE_CXX_COMPILER=/usr/bin/g++-9

run this in build folder we make in step2
```

#### step6:
```
1.make -j$(nproc)
2.sudo make install

```

### note : 
make sure both the step1 AND step2 should done seperatly


