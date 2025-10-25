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
<img width="818" height="618" alt="Screenshot 2025-10-24 202242" src="https://github.com/user-attachments/assets/48d85518-d07f-4a9b-b434-d283ead7a218" />


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
<img width="1281" height="801" alt="Screenshot 2025-10-24 214121" src="https://github.com/user-attachments/assets/0ced6b97-8831-4d06-b13a-68013f7d8321" />


### note : 
make sure both the step1 AND step2 should done seperatly

## Execution:
```
openroad -gui -log gcd_logfile.log gcd_nangate45.tcl
```
<img width="1257" height="801" alt="image" src="https://github.com/user-attachments/assets/e7006b5b-0f9f-4079-8e45-8693c7597134" />


## Reminder:
> i have problem with OpenROAD-Script file so i followed this procedure



