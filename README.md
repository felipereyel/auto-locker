# Auto Locker

Bash Script to automatically lock and unlock screensaver when specified USB device is plugged.

My personal use is for work.
I entered my phone's ID (captured with 'lsusb') and when I sit at my station to work and plug my phone it automatically unlocks and when I leave with my phone it unlocks.

Recommended to start with system startup.

My personal system runs with KDE Plasma 5.0 desktop. Some commands depend on the environment.

Commands:
 - `qdbus org.kde.screensaver /ScreenSaver org.freedesktop.ScreenSaver.GetActive` queries the current scrensaver state
 - `loginctl lock-session` locks the screen
 - `loginctl unlock-session` unlocks the screen

The programs runs in a while loop indefinitely, with 1 second sleep in between