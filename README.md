# volume
### Volume control and info script written in bash, written for PulseAudio.

#### Instructions:

0) `cd clone_location`
1) install pamixer from your distro package manager. also needs pactl.
2) `chmod +x volume; /usr/bin/install volume ~/home/$USER/.local/bin`

Commands:

`volume` to print the current volume
`volume up` to increase volume
`volume down` to decrease volume
`volume mute` to toggle volume muting
`volume muteon` to mute volume
`volume muteoff` to unmute volume

The script targets the sink with the highest number, i.e. the one plugged in most recently, so it automatically displays the volume of the sink that's currently being used. If no sink is currently running, it defaults to the lowest sink (0).
