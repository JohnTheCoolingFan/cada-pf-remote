I attempted replacing the micro usb plug for a type c plug in the receiver. Fortunately, I have found a type-c plug that matched pins with the micro usb plug (only needs GND and +5V, otehr pins don't even have pads on the board). Unfortunately, plugging the power in (with battery disconnected) caused one of the components to release the magic smoke. The board is basically dead now. The component that had visible damage is marked J3Y ([pdf datasheet](https://datasheet.lcsc.com/lcsc/1810161230_Jiangsu-Changjing-Electronics-Technology-Co---Ltd--S8050-J3Y_C2146.pdf)), which I think is a voltage regulator for one of the two ICs on the board besides the two 2-channel motor controllers.

I do not plan on repairing the board and will simply order anotehr remote control receiver brick, possibly from teh same seller I got it to start with. So this allowed me to go further in a semi-destructive breakdown of the board.

The board has 4 ICs, two of them being a MX1616 2-channel motor controller. The otehr two don't have markings on teh top, but do have markings on the bottom:
1. Marked `DY2003SLY1`, no information online. At the usb port side, pins facing the short sides of the board.
2. Marked `800[_ or 2]6K0805.1`, no information online. Unsure if I read the marking correctly. At the button side, pins facing the long sides of the board.

Since I did not find any information about these ICs online, I have no idea which one does what. Although, the second one has a quartz frequency generator near it and the antenna, so it might be responsible for wireless communication. `805.1` at the end might point in teh direction of teh protocol used, so sniffing with nRF24 might be a possibility.

(personal rambling below)

That's probably all I could identify on the board. Sad to lose the functionality for now, but I don't think I'm going to drive my 8x8 offroader in the snow.
