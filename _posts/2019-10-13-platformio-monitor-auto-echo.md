---
layout: post
title:  "Enable display of inputs inside Platformio Device Monitor"
---
The flag `--echo` enable the display of the inputs inside the *Platformio Monitor*.

This post explain how to activate it automatically.

1. Add inside `platformio.ini` this
```ini
[env:extra_monitor_flags]
platform = ...
board = ...
; The part to add
monitor_flags=
    --echo
```
2. You can now test if it work

## Resources
- [Monitor Options](https://docs.platformio.org/en/latest/projectconf/section_env_monitor.html#monitor-flags)
- [platformio device monitor](https://docs.platformio.org/en/latest/userguide/cmd_device.html#platformio-device-monitor)
