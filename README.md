# obliterate
Linux killswitch web app. Works as a panic button to wipe a computer remotely in emergency situations.

# Plan

## Client app

Can be configured to start on boot, check a web address periodically, obliterate the system when it finds a specific address (or when it doesn't) with a specific command (for example, wipe the LUKS header, or rm a certain file or directory), and optionally, reboot the system when done, kernel panic, etc.

## Server app

Will serve the necessary files for the client app to authenticate obliterations, and also can be used as a remote obliterator, because it can connect to specific hosts via SSH and run arbitrary commands there. The server is useful for instant destruction, whereas the client is useful as a fallback, in case SSH is firewalled or somehow doesn't work as expected.
