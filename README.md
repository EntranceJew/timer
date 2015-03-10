timer
=====
A simple lua timer library that mimics the [gmod timer library](http://wiki.garrysmod.com/page/Category:timer). 

Requirements
------------
- Lua >= 5.1

Usage
-----
timer, despite the name, doesn't track its own time. We have to provide it, making it ideal to live in a game loop:
```lua
function love.load()
	require('timer')
end

function love.update(dt)
	timer.Update(dt)
end
```
Once timer is being fed updates, the usage is basically the same as it is [for gmod](http://wiki.garrysmod.com/page/timer/Create).