# openHAB Smarther Widget

I've started working on this HABPanel widget for BTicino Smarther chronothermostat, as a companion to my [BTicino Smarther binding](https://community.openhab.org/t/bticino-smarther-thermostat-binding/73329).

Widget: [Smarther.widget.json](/widget/Smarther.widget.json) (13.2 KB)

## Main Panel

If the thermostat is off (left) or running its normal program (right), the widget looks like:

![OFF Status](/screenshots/screen1.png) ![ON Status](/screenshots/screen6.png)

Click the **hamburger** menu button (top-right), to access the Settings panel.

## Settings Panel

![Automatic Mode](/screenshots/screen3.png) ![Mode Selection](/screenshots/screen5.png) ![Manual Mode](/screenshots/screen2.png) ![Boost Mode](/screenshots/screen4.png)

Click the **power** button (top-right), to apply the new settings to the thermostat.

## Widget Configuration

The widget is configured setting the module base name and min/max temperature.
All the items needed to make the widget work are then derived from the module base name; for example, a module base name = `SMA_Thermo` implies that all the items reported in the config description (e.g. `SMA_Thermo_Sensor_Temperature`) must be defined in openHAB for the chronothermostat module you want to control:

![Widget Config](/screenshots/screen7.png)
