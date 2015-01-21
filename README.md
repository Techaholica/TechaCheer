# TechaCheer
Twitch bot which lets users enter commands that show pictures on the stream

To see this bot in action check out this article: http://techaholica.com/2015/01/10/check-out-my-twitch-overlay/

This bot will accept commands from the user and then show a picture representing that on the screen.
- !cheer - shows a happy me
- !boo - shows a sad me
- !love - shows a heart me

Your going to want to change the pictures in the TechaCheer directory so that my face doesn't show up on your stream. 

OBS setup instructions
- Add new picture scenes and specify that you want to check for updates.
- Choose the blank pictures labeled !boo_current.png, !cheer_current.png, and !love_current.png

Those pictures are blank so they won't show up on the stream, but when a user enters a command, the real picture is renamed to the _current.png file. Since you selected to check for updates on your scene, this picture will now show up on your stream. After a second the blank.png file is copied to the _current.png thus making it invible again. For every user that enters the command within a second of each other, the picture stays up for that long. So if five users enter !cheer, then the cheer picture will stay up for five seconds before going blank.

To install the script in mIRC, go the TechaCheer directory to %APPDATA%\mirc and then copy TechaCheer.ini to %APPDATA%\mirc\scripts.
