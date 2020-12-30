DisplayPort FIX
=====================

# Edited by Federico Giuggioloni

I forked the project to provided a much needed fix for displayport monitors: restore window position whenever the displayport monitor is turned on.

Currently hardcoded for my dual monitor setup: 3840x2160 (set as primary) and 1920x1080.
All the program does is:

- If the resolution was changed to 1920x1080, this means the displayport monitor was turned off -> Take a Snapshot
- If the resolution was changed to 3840x2160, this meand the displayport monitor was turned on -> Restore Snapshot (with a 5 second delay due to windows taking some time to reconfigure the new monitor)

Enjoy having a monitor that works the way it's supposed to!

## TODO

- Remove hardcoded resolutions.
- Find a way to avoid having to sleep before restoring snapshot
- If the sleep cannot be avoided, provide the user with a way to choose sleep amount in seconds


From https://github.com/adamsmith/WindowsLayoutSnapshot/issues/8:
Hi,

I see this project is not maintained for years.

But there are a lot of good forks, my suggestion is to select/create a new fork, and do all the changes from the other forks there.

Then create a community and so on.

See the forks here: https://techgaun.github.io/active-forks/index.html#https://github.com/adamsmith/WindowsLayoutSnapshot
