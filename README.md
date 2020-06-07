# volume
### Volume control and info script written in bash, for PulseAudio.

#### Dependencies

pamixer and pactl (so systemd, basically)

#### Instructions:

0) `git clone https://github.com/shantaram3013/volume`
1) `cd volume`
2) `/usr/bin/install volume ~/.local/bin` (or other binary directory of your choice)

Commands:

`volume` to print the current volume    
`volume up` to increase volume    
`volume down` to decrease volume    
`volume mute` to toggle volume muting    
`volume muteon` to mute volume    
`volume muteoff` to unmute volume    
   
The script targets the sink with the highest number, i.e. the one plugged in most recently, so it automatically displays the volume of the sink that's currently being used. If no sink is currently running, it defaults to the lowest sink (0).
