# xrandr

display information about all connected screens

    xrandr


duplicate screen on all available displays (reset to default when only one
screen is available)

    xrandr --auto


duplicate the DP screen on the HDMI screen

    xrandr --output HDMI1 --same-as eDP1 --auto


add the HDMI screen on the right of the DP screen

    xrandr --output HDMI1 --right-of eDP1 --auto


same, but explicitly set mode

    xrandr --output HDMI1 --right-of eDP1 --mode 1680x1050


turn of the HDMI output

    xrandr --output HDMI1 --off


# Basic Usage

    xrandr --output <screen1> --<position> <screen2> --auto

* `<position>` can be any of `left-of`, `right-of`, `above`, `below` or
  `same-as`
* screens are typically `HDMI1`, `VGA1`, `eDP1` or `DVI1`, see the output of
  `xrandr` to know what outputs are available for you


