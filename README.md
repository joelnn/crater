# crater
crater is a simple shell `exec` wrapper for installing Lua and LuaRocks.

You can:
* Specify every option:    
`CRATER_ROOT="$(pwd)/.crater" CRATER_LUA=lua-5.3.0 CRATER_LUAROCKS=luarocks-2.2.2 crater lua`  
* Use the defaults, or the last specified versions, in the default root:  
`crater lua`
* Source crater to modify your PATH, allowing you to invoke lua/luarocks or run scripts with `#!/usr/bin/env lua` shebangs thereafter:  
`CRATER_ROOT="$(pwd)/.crater" CRATER_LUA=lua-5.3.0 CRATER_LUAROCKS=luarocks-2.2.2 . crater` 
