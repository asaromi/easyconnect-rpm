# Manual Install EasyConnect VPN on RPM-based Linux

### 1. Download your .rpm installer
Download your npm installer from a trusted source (like me downloading from my company address - EasyConnect_x64_7_6_7_3.rpm)

### 2. Install the package
Run command `sudo rpm -i /path/to/easyconnect.rpm`

### 3. Open the EasyConnect App
If you try to open the app or run the commands below

`cd /usr/share/sangfor/EasyConnect/`

`./EasyConnect`

### 4. It's not working yet when opening the app? Don't worry
You need these 3 packages: `libpango-1.0`, `libpangocairo-1.0`, `libpangoft2-1.0`. Download it from the current repo (FYI the libpango was downloaded from pango-1.42)
Then compress and copy all lib files to `/usr/share/sangfor/EasyConnect/`

`cp -rf /path/to/downloaded/packages/libpango* /usr/share/sangfor/EasyConnect/`

You can now open EasyConnect from the desktop, and it should start up correctly.


## References
- https://www.wannaexpresso.com/en-us/2020/06/07/easy-connect-manjaro/
- https://www.cnblogs.com/cocode/p/12890684.html
