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

iframe:
    widget_type: iframe
    refresh: 1800
    img_list:
      - http://decoholic.org/wp-content/uploads/2014/12/scandinavian-design-1.jpg
      - http://cdn.freshome.com/wp-content/uploads/2014/01/6-Series-7-Scandinavian-Design.jpg
      - http://www.greatwallart.com/wp-content/uploads/2016/04/swedish-design-3-scandinavian-design-also-typical-scandinavian-light-interior-images-scandinavian-interior-design.jpg
      - http://www.contemporist.com/wp-content/uploads/2016/07/scandinavian-interiors_140716_01-800x420.jpg
      - http://cdn.homedit.com/wp-content/uploads/2015/04/Minimal-wood-treatment.jpg

layout:
    - iframe(8x5)
    - spacer(8x1)
    - spacer(8x1)
    - spacer(8x1)
    - spacer(8x1)
    - include: bottom_panel
```

It seems like pictures are rendered correctly even without the google proxy.
If this is not the case on your machine, change the `img_list` like this:
```
https://images1-focus-opensocial.googleusercontent.com/gadgets/proxy?url=http://cdn.homedit.com/wp-content/uploads/2015/04/Minimal-wood-treatment.jpg&container=focus&refresh=240&resize_h=640&resize_h=640
```
