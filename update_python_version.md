## Follow the below process to set the default version of python3 as python3.9 in jetson nano

Firstly, install the python version that you need:
For python3.9 install using: **sudo apt-get install python3.9**

1. sudo update-alternatives --config python3
2. sudo update-alternatives --install /usr/bin/python3 python /usr/bin/python3.9 1
3. sudo update-alternatives --install /usr/bin/python3 python /usr/bin/python3.6 2
4. sudo update-alternatives --config python3

or use 

4. sudo update-alternatives  --set python3 /usr/bin/python3.9

### Also install the following:
sudo apt install python3.9-distutils

Useful links:

https://stackoverflow.com/questions/71034111/how-to-set-default-python3-to-python-3-9-instead-of-python-3-8-in-ubuntu-20-04-l

https://askubuntu.com/questions/1292972/importerror-cannot-import-name-sysconfig-from-distutils-usr-lib-python3-9
