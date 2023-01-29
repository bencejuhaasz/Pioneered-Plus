# Pioneered-Plus
Pioneer DJ-style extension pack for open source DJ software Mixxx (https://github.com/mixxxdj/mixxx)
Turn your controller into a standalone deck with any linux-compatible device and a touch screen !
(https://www.youtube.com/watch?v=IkuiykgW858, https://www.youtube.com/watch?v=kyrJW7Vaf68)
Big thanks Sven Boekelder, aka @timewasternl for creating the awesome skin I'm building on.
(Only reason I'm not forking is new folder structure)

# Features
* Pioneer-style effect chain pack, both for BEAT FX and COLOR FX, with corresponding names and sound profiles
* CDJ/XDJ-like user interface created for touch screens
* Rekordbox USB support: export your library in rekordbox, plug in your USB key into your linux device, and play as you would on a CDJ/XDJ setup. Hotcues, key and bpm info is recognized. If you've used Mixed In Key, you'll find the extra info in `comments` in library view.
* Corresponding MIDI mapping and js plugin (for DDJ-400 at the time of writing, with all pad modes implemented)

# Install
* 1.: Copy everything into `~/.mixxx`
* 2.: In preferences, select `Pioneered` for MIDI controller profile, set up your soundcard, in effects in the left panel delete everything except the chains starting with `B_`, in the right panel delete everything except chains starting with `C_` (this way you can cycle through color effects via left and right on beatfx panel, and through beat effects via down arrow. the first effect on the left panel will be your first pad fx and so on), set crossfader for scratching if you'd like, in key detection set format to `Lancelot` to use same format as Rekordbox does to avoid confusion. In decks set hotcue mode to Pioneer and tempo range how you'd like. Don't forget to set required track info in library mode via right clicking on the column names.
* 3.: Have fun DJ'ing:)

# Infos
* Rekordbox USB's need to be mounted at /media/your username/SOMETHING-XX
* If you're using a raspberry pi, I recommend DietPi OS and then installing openbox to minimize software bloat. Feel free to use the provided desktop file, for autostart put it into `~/.config/autostart/` . It requires sudo, but it changes real time priority and gets rid of the otherwise present ui lags. 

# Requirements
* Mixxx built from latest master branch (2.4 alpha)
* Touch screen (will work otherwise, but not as intended)
* DDJ-400 (will work otherwise, but not as intended)
