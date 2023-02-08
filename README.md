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
In the `.bashrc` file include the follow line with your directory:
 ```
 export LD_LIBRARY_PATH=/home/fcost/libpng12/lib/i386-linux-gnu
 ```
  5. If you are using the 22.04 LTS version of Ubuntu, you will probably have to do this;
  ```
  sudo apt-get install libfontconfig1:i386
  ```
  6. You have to edit the `.bashrc` file again with;
  ```
  export PATH=/home/fcost/altera/13.0sp1/quartus/bin:$PATH
  ```
  7. For more explanations, you can find [here](https://www.youtube.com/watch?v=T-Tg2uEuX6o) (**It's in portuguese**);
  
  8. The `fcost` is my username, you must change for your.
