# [Hygge](https://en.wikipedia.org/wiki/Hygge) Theme for [HA Dashboard](https://home-assistant.io)!

First attempt creating a puristic color theme for the second version of [HA Dashboard](https://github.com/home-assistant/appdaemon/blob/master/DASHBOARD.md).


# Preview

![Screenshot 1](img/screen1.png?raw=true)

![Screenshot 2](img/screen2.png?raw=true)

# Installation

Add the skin to the `custom_css` folder:
```sh
git clone https://github.com/JulianKahnert/hygge.git /PATH/TO/custom_css/hygge
```

Start your Hygge-Dashboard:
```
http://<ip address>:<port>/<dashboard name>?skin=hygge
```

# Example Screensaver Configuration

```
#
# Main arguments, all optional
#
title: Screensaver
widget_dimensions: [120, 120]
widget_size: [1, 1]
widget_margins: [5, 5]
columns: 8
global_parameters:
    use_comma: 0
    precision: 1
    use_hass_icon: 1

layout:
    - spacer(8x1)
    - spacer(8x1)
    - spacer(8x1)
    - spacer(8x1)
    - spacer(8x1)
    - include: bottom_panel
```
