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
5. Remove the file `libxcb-dri3.so.0` in `~/ROBOTIS/DynamixelWizard2`
