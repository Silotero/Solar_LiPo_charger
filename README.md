# Solar_LiPo_charger
Solar panel battery charger

This is a battery charger that uses solar panels for the charging. It has a max charging input to the batteries of 4 A. It is also capable of outputing up to 15W of power at 5V 3A at its USB-C port. It also has a screw terminal with the same output capabilities.

The charging IC that takes care of taking the solar input (which must be 2 panels in series, the rest, up to 20 of such pairs, in parallel), making the constant-current/constant-voltage work is the CN3791. The IC responsible for making sure that the batteries don't get overcharged, overdischarged or shorted is the AP9101CK6. It also uses the PAM2423 boost converter to achieve the 5V output on the screw terminal as well as the USB-C port. The announcement of the USB-C capabilities is done via 10k ohm resistors pulled up to VCC on the CC pins.
