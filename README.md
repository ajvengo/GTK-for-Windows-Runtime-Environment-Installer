GTK+ for Windows Runtime Environment Installer: 64-bit
======================================================

This repository is a fork of the  [GTK+ for Windows Runtime Environment Installer](http://gtk-win.sourceforge.net) that was originally created
by Alexander Shaduri.
My efforts here will focus on creating a **64-bit version** of the GTK+-2 runtime that he has been providing so far, using up to date versions of GTK+ and its dependencies. Recently I have also created a 64-bit **GTK+-3 runtime package**. All packages now contain **Gtkmm** and its dependencies too. Since the GTK+ developers recently dropped support for stock icons (a mistake of epic proportions IMHO...), I added the Gnome icon theme to the GTK+-3 runtime, so you can still enjoy pretty filechooserdialogs etc!

The installers can be found [here](http://lvserver.ugent.be/gtk-win64/).

**[Keep in mind though that these packages are experimental. Binary compatibility between versions is not guaranteed!!!.](http://www.gtk.org/download/win64.php)** 

Both for convencience as well as for increased reliability across installations, it is recommended for developers to compile and link against the GTK+ SDK that I used to create the installers. This SDK can also be obtained at the aforementioned url.

The current releases ([gtk2-runtime-2.24.25-2015-01-21-ts-win64.exe](http://lvserver.ugent.be/gtk-win64/gtk2-runtime/gtk2-runtime-2.24.25-2015-01-21-ts-win64.exe) and [gtk3-runtime-3.14.7-2015-01-27-ts-win64.exe](http://lvserver.ugent.be/gtk-win64/gtk3-runtime/gtk3-runtime-3.14.7-2015-01-27-ts-win64.exe)) has been compiled using GCC 4.9.2 (MinGW-w64 installed from TDM-GCC).
The included GTK+ dependencies were selected according to the flowchart used by [Hexchat](http://hexchat.github.io/gtk-win32/). The source tarballs can be obtained by clicking on the names of the dependencies in the following list:

* [atk](http://ftp.gnome.org/pub/GNOME/sources/atk/) (2.14.0)
* [atkmm](http://ftp.gnome.org/pub/GNOME/sources/atkmm/) (2.22.7)
* [cairo](http://cairographics.org/releases/) (1.14.0)
* [cairomm](http://cairographics.org/releases/) (1.11.2)
* [fontconfig](http://www.freedesktop.org/software/fontconfig/release/) (2.11.1)
* [freetype](http://www.freetype.org/download.html) (2.5.5)
* [gdk-pixbuf](http://ftp.gnome.org/pub/GNOME/sources/gdk-pixbuf/) (2.30.8)
* [gettext](http://ftp.gnu.org/pub/gnu/gettext/) (0.19.4)
* [glib](http://ftp.gnome.org/pub/GNOME/sources/glib/) (2.42.1)
* [glibmm](http://ftp.gnome.org/pub/GNOME/sources/glibmm/) (2.42.0)
* [gnome-icon-theme](http://ftp.gnome.org/pub/GNOME/sources/gnome-icon-theme/) (3.12.0)
* [gnome-icon-theme-extras](http://ftp.gnome.org/pub/GNOME/sources/gnome-icon-theme-extras/) (3.12.0)
* [gnome-icon-theme-symbolic](http://ftp.gnome.org/pub/GNOME/sources/gnome-icon-theme-symbolic/) (3.12.0)
* [gtk2](http://ftp.gnome.org/pub/GNOME/sources/gtk+/) (2.24.25)
* [gtk3](http://ftp.gnome.org/pub/GNOME/sources/gtk+/) (3.14.7)
* [gtkmm2](http://ftp.gnome.org/pub/GNOME/sources/gtkmm) (2.24.4)
* [gtkmm3](http://ftp.gnome.org/pub/GNOME/sources/gtkmm) (3.14.0)
* [harfbuzz](http://www.freedesktop.org/software/harfbuzz/release/) (0.9.37)
* [hicolor-icon-theme](http://icon-theme.freedesktop.org/releases/) (0.14)
* [icon-naming-utils](http://tango.freedesktop.org/releases/) (0.8.90)
* [intltool](http://ftp.gnome.org/pub/gnome/sources/intltool/) (0.50.2)
* [libffi](http://sourceware.org/libffi/) (3.2.1)
* [libpng](http://sourceforge.net/project/showfiles.php?group_id=5624) (1.6.16)
* [libsigc++](http://ftp.gnome.org/pub/GNOME/sources/libsigc++/) (2.4.0)
* [libxml2](http://xmlsoft.org/sources/) (2.9.2)
* [pango](http://ftp.gnome.org/pub/GNOME/sources/pango/) (1.36.8)
* [pangomm](http://ftp.gnome.org/pub/GNOME/sources/pangomm/) (2.34.0)
* [pixman](http://cairographics.org/releases/) (0.32.6)
* [win-iconv](http://code.google.com/p/win-iconv/downloads/list) (0.0.6)
* [zlib](http://www.zlib.net) (1.2.8)

For all other information regarding how to use the installer, the reader is kindly referred to the [Alexander Shaduri's website](http://gtk-win.sourceforge.net) of the GTK for Windows runtime environment installer. The only difference with the installers found at this website is that mine DO NOT have the `compatdlls` option, but this should present no problems to any user.  

Personally I use this installer in my [XMI-MSIM project](http://github.com/xmimsim). You may want to have a look at my Inno Setup ([new](https://github.com/tschoonj/xmimsim/blob/master/nsis/xmimsim.iss)) and NSIS ([old](https://github.com/tschoonj/xmimsim/blob/XMI-MSIM-4.0/nsis/xmimsim-win64.nsi.in)) based installers. 


Tom Schoonjans
