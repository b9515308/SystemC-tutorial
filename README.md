# SystemC tutorial

## Whats is SystemC

SystemC is a set of classes and libraries that provide event driven simulation. SystemC is based on C++, which gives it speed and flexibility.

Being based on C++, SystemC doesnt require any special EDA tool in order to use it. All you need is a C++ compiler that you can link your installation to.

Knowledge of C++ is required in order to understand this.

## Instalation

Dependencies:

- For Debian/Ubuntu and Ubuntu based distros
```
sudo apt install build-essential make wget
```

- For Arch, Manjaro and other Arch based distros
```
sudo pacman -S gcc make wget
```
- For Red Hat and CentOS
```
sudo yum groupinstall "Development Tools"
sudo yum install kernel-devel kernel-headers wget
```

SystemC can be downloaded, free of charge, from Accellera's website.

Steps:
1. Open terminal and type
```
wget http://www.accellera.org/images/downloads/standards/systemc/systemc-2.3.2.tar.gz
```
This downloads the SystemC tarball

2. Unpacking the package and making directories
```
tar -xzf systemc-2.3.2.tar.gz
sudo mkdir /usr/local/systemc-2.3.2
cd systemc-2.3.2 && mkdir objdir && cd objdir
```

3. Final installation
```
sudo ../configure --prefix=/usr/local/systemc-2.3.2/
sudo make
sudo make install
```
