alarmscript
===========

Simple linux alarm script. Is supposed to be run via cron. Requires alsa and mplayer installed.

<h2>Description of the files:</h2>
 - <b>incvolume.sh</b> mutes / unmutes sound; gradually increases volume over time. for information on your channels please use alsamixer utility
 - <b>play.sh</b> launches mp3 player in X11 terminal window with the specified playlist
 - <b>AlarmSongs.m3u</b> sample playlist; use your own instead

<h2>How to schedule script execution via cron:</h2>
<tt>30 7 * * * { <i>full_path_to_script</i>/incvolume.sh& } && <i>full_path_to_script</i>/play.sh</tt>
