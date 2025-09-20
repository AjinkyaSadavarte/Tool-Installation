# Tool-Installation
Task 1 and Task 2 for documentation and installation of tools\
# 1. Yosys Installation
```
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make (If make is not installed please install it)
$ sudo apt-get install build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 libboost-system-dev \
libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
$ make
$ sudo make install
```
<img width="1748" height="1433" alt="image1" src="https://github.com/user-attachments/assets/3d722bf9-19e0-442d-943f-f2df45cc9829" />

# 2. Iverilog
```
sudo apt-get update
sudo apt-get install iverilog
```
<img width="1748" height="512" alt="Screenshot from 2025-09-20 23-32-27" src="https://github.com/user-attachments/assets/4e36d659-c2fd-4a87-a309-dd22e02f921d" />

# 3. GTKWave
```
sudo apt-get update
sudo apt install gtkwave
```
<img width="1748" height="366" alt="Screenshot from 2025-09-20 23-35-21" src="https://github.com/user-attachments/assets/5c7da615-bd0a-42e9-ba81-c36b6d7b2111" />
<img width="3190" height="2000" alt="Screenshot from 2025-09-20 23-36-12" src="https://github.com/user-attachments/assets/466fb060-217a-4c70-b46e-12535fb3871e" />

# 4. ngspice
After downloading the tarball from https://sourceforge.net/projects/ngspice/files/ to a local
directory, unpack it using:
```
$ tar -zxvf ngspice-37.tar.gz
$ cd ngspice-37
$ mkdir release
$ cd release
$ ../configure --with-x --with-readline=yes --disable-debug
$ make
$ sudo make install

```
<img width="1721" height="662" alt="Screenshot from 2025-09-20 23-46-21" src="https://github.com/user-attachments/assets/59e0f3cd-5421-4669-8534-a2f025944245" />

# magic

```
$ sudo apt-get install m4
$ sudo apt-get install tcsh
$ sudo apt-get install csh
$ sudo apt-get install libx11-dev
$ sudo apt-get install tcl-dev tk-dev
$ sudo apt-get install libcairo2-dev
$ sudo apt-get install mesa-common-dev libglu1-mesa-dev
$ sudo apt-get install libncurses-dev
git clone https://github.com/RTimothyEdwards/magic
cd magic
./configure
make
make install
```
<img width="3026" height="1930" alt="Screenshot from 2025-09-20 23-48-20" src="https://github.com/user-attachments/assets/1e74bd78-b592-4a3a-803d-e370041c2f41" />


# OpenLANE
```
sudo apt-get update
sudo apt-get upgrade
sudo apt install -y build-essential python3 python3-venv python3-pip make gitsudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o
/usr/share/keyrings/docker-archive-keyring.gpg
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg]
https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee
/etc/apt/sources.list.d/docker.list > /dev/null
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io
sudo docker run hello-world
sudo groupadd docker
sudo usermod -aG docker $USER
sudo reboot
```
After reboot, do the following
```
docker run hello-world
```





