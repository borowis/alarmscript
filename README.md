alarmscript
===========

Simple linux alarm script. Is supposed to be run via cron. Requires alsa and mplayer installed.

Description of the files:
 - incvolume.sh mutes / unmutes sound; gradually increases volume over time. for information on your channels please use alsamixer utility
 - play.sh launches mp3 player in X11 terminal window with the specified playlist
 - AlarmSongs.m3u sample playlist; use your own instead

How to schedule script execution via cron:
30 7 * * * { <full path to script>/incvolume.sh& } && <full path to script>/play.sh
