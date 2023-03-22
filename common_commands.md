# Common Commands
To retain any of these settings after closing/reopening CSGO, move the command(s) from this file to `C:\Steam\steamapps\common\Counter-Strike Global Offensive\csgo\cfg`
### Table of contents
- [Netgraph](#netgraph)
- [Hud & Radar](#hud)
- [Movement binds](#movement)
- [Audio](#audio)
- [Faceit](#faceit)

<a name="netgraph"></a>

## Net graph
Toggles netgraph on, which shows FPS, ping, and tick rate. 
```
net_graph 1
```
Bind netgraph to show when pressing tab / hide when let go
```
bind "TAB" "+ng"
alias "+ng" "+showscores; net_graph 1"
alias "-ng" "-showscores; net_graph 0"
```
<a name="hud"></a>

## Team
Centers the radar, allowing you to see a majority of the map
```
cl_radar_always_centered
```
Allows you to see your teammate’s weapons and utility
```
cl_show_team_equipment
```

<a name="movement"></a>

## Movement binds
Bind scroll wheel up/down to jump
```
bind mwheelup +jump;bind mwheeldown +jump;bind space +jump
```
<a name="audio"></a>

## Audio
Enable 10 second round end music warning - useful to know whether or not you can stick a defuse with no kit
```
snd_roundend_volume 1.0
```
<a name="faceit"></a>

## Faceit
Fixes lag / stuttering encountered on faceit servers
```
logaddress_add 1
```
