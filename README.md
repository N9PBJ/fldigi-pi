# fldigi-pi
Instructions for installing fldigi on raspberry pi

* Make sure pi is up to date:
```sh
sudo apt update
sudo apt upgrade -y
```

* Remove existing fldigi installed from offical repos if it exists:  
```sh
sudo apt remove fldigi --purge
```

* Install the required libraries for fldigi:  
```sh
sudo apt build-dep fldigi
```
* Download the latest fldigi:
  * http://www.w1hkj.com/
  * You want the one that ends in .tar.gz

* Extract the files in a terminal  
```sh
cd ~/Downloads
tar -zxvf <name-of-file-downloaded>.tar.gz
```

* Run the auto-configuration tool  
```sh
cd fldigi<tab-key>
./configure
```

* Compile the program:  
```sh
make
```

* Install the program:
```sh
sudo make install
```

* Launch and put process in background:
```sh
fldigi &
```
