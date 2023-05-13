## Follow the below process to set the default version of python3 as python3.9 in jetson nano

1. sudo update-alternatives --config python3
2. sudo update-alternatives --install /usr/bin/python3 python /usr/bin/python3.9 1
3. sudo update-alternatives --install /usr/bin/python3 python /usr/bin/python3.6 2
4. sudo update-alternatives --config python3

or use 

4. sudo update-alternatives  --set python3 /usr/bin/python3.9

### Also install the following:
sudo apt install python3.9-distutils

