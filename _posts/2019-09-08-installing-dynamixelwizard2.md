---
layout: post
title:  "Installing DynamixelWizard2 on Ubuntu"
ref: install-dynamixelwizard2
lang: en
---

This is how you can install DynamixelWizard2 on Ubuntu.

1. Download `DynamixelWizard2Setup_x64` from [ROBOTIS website](http://emanual.robotis.com/docs/en/software/dynamixel/dynamixel_wizard2/#software-installation)
2. Make the setup file executable `sudo chmod u+x DynamixelWizard2Setup_x64`
3. Run `./DynamixelWizard2Setup_x64`
4. Follow the installation step

If you get the following error:
```
DynamixelWizard2: symbol lookup error: /usr/lib/x86_64-linux-gnu/libGLX_mesa.so.0: undefined symbol: xcb_dri3_get_supported_modifiers
```
5. Remove the file `libxcb-dri3.so.0` in `~/ROBOTIS/DynamixelWizard2`

You can now use DynamixelWizard2.
