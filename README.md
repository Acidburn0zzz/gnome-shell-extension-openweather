# Weather Extension V2 (<= GNOME Shell 3.8)

![Screenshot](https://f.cloud.github.com/assets/1255506/833069/0f754966-f28b-11e2-9fb3-3ea413919c69.png)

*gnome-shell-extension-weather* is a simple extension for displaying weather conditions and forecasts in GNOME Shell, featuring support for multiple locations, no need for WOEID, a symmetrical layout and a settings panel through *gnome-shell-extension-prefs*.

The weather report include forecasts for ~ 10 days.

----

# Installation

Make sure you have the following dependencies installed:
* *gettext*,
* *pkg-config*,
* *git*,
* *glib2*,
* *glib2-devel* or *libglib2.0-dev*,
* *zip*,
* *gnome-common*,
* *autoconf*,
* *automake*,
* *intltool*.

Run the following commands:

	cd ~ && git clone git://github.com/Neroth/gnome-shell-extension-weather.git
	cd ~/gnome-shell-extension-weather
	./autogen.sh && make local-install

Restart GNOME Shell (`Alt`+`F2` => `r` => `Enter`) and enable the extension through *gnome-tweak-tool*.

----

# Configuration

Launch *gnome-shell-extension-prefs* (reachable also through the *Weather Settings* button on the extension popup) and select *Weather* from the drop-down menu to edit the configuration.

![Screenshot](https://github.com/neroth/gnome-shell-extension-weather/raw/master/data/weather-settings.gif)

You can also use *dconf-editor* or *gsettings* to configure the extension through the command line.

----

# Debug

To debug the extension, active the switch `Debug extension` in the settings:

You have now two new file ("weather.log" and "weather-prefs.log") in the extension dir (`~/.local/share/gnome-shell/extensions/weather-extension@xeked.com/`).

----

# Licence

Copyright (C) 2011 - 2013

* Christian Metzler <neroth@xeked.com>,
* Elad Alfassa <elad@fedoraproject.org>,
* Mark Benjamin <weather.gnome.Markie1@dfgh.net>,
* Simon Claessens <gagalago@gmail.com>,
* Ecyrbe <ecyrbe+spam@gmail.com>,
* Timur Kristóf <venemo@msn.com>,
* Simon Legner <Simon.Legner@gmail.com>,
* Mattia Meneguzzo <odysseus@fedoraproject.org>.

This file is part of *gnome-shell-extension-weather*.

*gnome-shell-extension-weather* is free software: you can redistribute it and/or modify it under the terms of the **GNU General Public License as published by the Free Software Foundation, either version 3** of the License, or (at your option) any later version.

*gnome-shell-extension-weather* is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with *gnome-shell-extension-weather*.  If not, see <http://www.gnu.org/licenses/>.
