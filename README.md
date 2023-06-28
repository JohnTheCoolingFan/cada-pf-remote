# cada-pf-remote

This repository is used to collect information about CaDA's 2.4GHz remote control for lego power functions compatible motors.

The receiver brick has a built-in accumulator and is charged through usb. CaDA product codes are: JV1010 for white 500mAh, JV1031 for white 750mAh

Remote has 4 controls, color-coded to match the receiver. Product code is JV8011. All controls have little real-life travel but only 3 states: forward, backward, off. Making better control options is one of the reasons for the start of this data collection.

CaDA's remote control uses some frequency in the range of 2.4GHz, like bluetooth or wifi, but it does not show up on a smartphone with regular tools. The chip inside the remote doesn't have any markings (either erased or never put on), and it's a single chip in teh entire controller, so it is not possible to sniff spi between controller chip and radio chip.

Possible investigation directions:
- [ ] use more sophisticated software tools to scan for bluetooth and wifi signals
- [ ] capture radio data and attempt to decode it
