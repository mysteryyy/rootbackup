
#!/bin/bash
a=$(awk -F"[][]" '/dB/ { print $2 }' <(amixer sget Master))
vol=$(echo $a | tr -dc '0-9')
if [ $vol -lt 90 ]
then
    
    amixer set 'Master' 100%
fi

mplayer -loop 0 /home/sahil/Downloads/alarm.mp3


