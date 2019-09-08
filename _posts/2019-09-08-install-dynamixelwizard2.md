---
layout: post
title:  "Install DynamixelWizard2 on Ubuntu"
date:   2019-09-08
---
This article is for the person that get the following error when trying to open DynamixelWizard2.

```
./ROBOTIS/DynamixelWizard2/DynamixelWizard2: error while loading shared libraries: libQt5AutoUpdaterGui.so.2: cannot open shared object file: No such file or directory
```

1. Download `DynamixelWizard2Setup_x64` from [ROBOTIS website](http://emanual.robotis.com/docs/en/software/dynamixel/dynamixel_wizard2/#software-installation)
2. Make the setup file executable `sudo chmod u+x DynamixelWizard2Setup_x64`
3. Run `./DynamixelWizard2Setup_x64`
4. Follow the installation step
5. Add `DynamixelWizard2` folder to the lib path
```bash
sudo sh -c "echo '/home/jonathan/ROBOTIS/DynamixelWizard2/' >> /etc/ld.so.conf.d/dynamixel.conf"
```
8. Apply the change `sudo ldconfig`
9.  Finally, launch `./ROBOTIS/DynamixelWizard2/DynamixelWizard2`