# Quackcordia

This is a personal fork of [SinisterRectus/Discordia](https://github.com/SinisterRectus/Discordia), adding personal improvments and changes used in [Ducky](https://duckybot.xyz/).


## Memory-Safe Options (Quackscordia-lean)

These options reduce idle RAM significantly without breaking the API:

```lua
local client = Client({
  weakUsers = true,      -- use weak cache for global users (default: true)
  weakMembers = true,    -- use weak cache for guild members (default: true)
  enableVoice = true,    -- set to false to avoid loading voice stack at startup
  cacheAllMembers = false, -- keep this false unless you really need full rosters
  -- gatewayIntents = ...  -- prefer the minimal set your bot needs
})
```
