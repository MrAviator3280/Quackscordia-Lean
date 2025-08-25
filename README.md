# Quackcordia

This is a personal fork of [SinisterRectus/Discordia](https://github.com/SinisterRectus/Discordia), adding personal improvments and changes used in [Ducky](https://duckybot.xyz/).


## Quacksdordia-lean

A fork of [DuckySupport/Quackscordia](https://github.com/DuckySupport/Quackscordia)

Less Memory Usage compared to Quackscordia (we hope)

Message Cache Capping via:
```lua
local client = discordia.Client({
    messageLimit = 100  -- cap cached messages per channel; off if nil/0/omitted
})
```
