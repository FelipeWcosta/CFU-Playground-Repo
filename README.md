# CFU-Playground-Repo
 Next step: Add the Quartus toolchain to the PATH
  1. Update and upgrade of all packages;
  2. Install dependeces of 32 bits kernel; 
   ```
   sudo apt install -y libstdc++6:i386 libc6:i386 libx11-dev:i386 libxext-dev:i386 libxau-dev:i386 libxdmcp-dev:i386 libfreetype6:i386 expat:i386 libxrender1:i386 libsm6:i386
   ```
  3. Download the Quartus II web version [here](https://www.intel.com/content/www/us/en/software-kit/666221/intel-quartus-ii-web-edition-design-software-version-13-1-for-windows.html);
  4. Install the library libpng12 with;
  ```
  wget https://launchpad.net/~ubuntu-security/+archive/ubuntu/ppa/+build/15108507/+files/libpng12-0_1.2.54-1ubuntu1.1_i386.deb
  ```
  ```
  dpkg -x libpng12-0_1.2.54-1ubuntu1.1_i386.deb libpng12
  ```
In the bin Quartus folder you must to do:
 ```
 export LD_LIBRARY_PATH=/home/libpng12/lib/i368-linux-gnu
 ```
