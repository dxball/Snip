Snip v2.0
by David Rudie (d.rudie@gmail.com)

This is a small application that sits in the system tray and updates a text
file with the currently playing audio track.

It supports Spotify, iTunes, and WinAmp.

If you choose to use iTunes then Snip will automatically launch iTunes.  This
is the behavior of the COM API and there's nothing I can do about it.  If you
only use Spotify then you don't have to worry about it.

To switch between players just right-click on the icon in the system tray.

Snip will write a generic format output to a file called Snip.txt within the
same folder as Snip.exe.  If you choose to save information to separate files
then the files will be called Snip_Arist.txt, Snip_Track.txt, Snip_Album.txt,
and if you choose to save track history then it will be saved to a file
called Snip_History.txt.

There are also some hotkeys implemented that can be used to do various things:
Next Track: Ctrl, Alt, ]
Previous Track: Ctrl, Alt, [
Volume Up: Ctrl, Alt, +
Volume Down: Ctrl, Alt, -
Mute Track: Ctrl, Alt, M
Play/Pause Track: Ctrl, Alt, Enter
Stop Track: Ctrl, Alt, Backspace

Not all hotkeys work between Spotify, iTunes, and WinAmp.


Changes

v2.0 (2013-Jan-17):
* Prior change in v1.6.5 that I forgot to mention:
    Snip now defaults to have most options disabled by default.
* WinAmp support added.
* Added the ability to save album information.

v1.6.5 (2013-Jan-4):
* Fixed a bug preventing output format working with iTunes.
* Added code to make sure only one instance of Snip can run at once.

v1.6 (2013-Jan-1):
* Added the ability to set a custom output format.
    If you save the track and artist information to separate files then make
    sure the separator that you use does NOT appear in any track or artist
    title.  If it does then the text will not get separated correctly.
* Expanded the memory range that Snip searches for the track information.

v1.5 (2012-Nov-11):
* Snip_Artist.txt and Snip_Track.txt will now be written.  These can be used
    to display the artist or track name in different styles.
* Added support for saving image artwork.  Spotify's support is rather hacky
    so it may not always work, or it may cause Spotify to randomly stop
    playing music.

v1.1.1 (2012-Sep-14):
* Fixed Snip_History.txt to use Environment.NewLine instead of \n.

v1.1 (2012-Sep-14):
* Added support for saving track history.
    This will save the history to a new text file called Snip_History.txt.

v1.0 (2012-Aug-12):
* Initial Release
