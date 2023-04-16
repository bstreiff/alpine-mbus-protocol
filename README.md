_**NOTE FROM 2023:** This was a project from 2009. I do not expect to get
back to it-- I've not had the vehicle I intended it for in nearly a decade.
My guess is that there aren't many other people out there looking for
protocol documentation for the sixth-gen Civic headunits, but I'm throwing
this up just in case it might be your lucky day._

# Alpine M-Bus Protocol

## Overview

When I purchased my 1996 Honda Civic, I inherited an okay aftermarket stereo
with it, but unfortunately it offered no aux-in for connecting an MP3 player
(such as the iPod mini that I
[upgraded with a 16GB CompactFlash card](https://web.archive.org/web/20080204223732/http://geektechnique.org/projectlab/759/the-ipod-mini-remastered-now-with-16gb)
but has been sitting idle since I got an iPhone). I bought a FM transmitter,
but the audio quality is bad and I have to manually start and stop the iPod
because the power outlet is only on when the car is on, and my iPod no longer
has the battery capacity to continue playing all day sitting in my parked car.
So, I did some research.

The previous owner replaced the stock radio because it was just a radio--
no tape deck, no CD player. On that year (and I believe the 1997 and 1998
models as well) there was an optional tape deck or CD player module that
mounted at the base of the dash. (There's just an empty slot in my car,
because it's pretty much the base model. Power locks? Power windows? Cruise
control? What are these things you speak of?)

And if there's an optional module for some sort of slave device,
than the stock radio must have some sort of means to connect the two! Also
having the stock radio would be a lot more convenient-- playing the 'I need
to detach my faceplate so that someone doesn't try to jack my aftermarket
stereo system!' is only fun for so long.

More research indicated that the stock headunits were manufactured by
[Alpine](http://www.alpine-usa.com/), and use a protocol
known both as 'M-Bus' and 'Versatile M-Link' (NOT Ai-Link; that's a
different one). Some work to reverse-engineer the protocol had also already
been done by [Joerg Hohensohn](https://web.archive.org/web/20220301142108/http://www.hohensohn.info/mbus/)
and [Hone Heke](https://web.archive.org/web/20120318034806/http://kiora.ath.cx/alpine).
This plan might have a shot at working. I picked up the stock headunit for
my car from eBay, for about $30.

My goal: Get an Arduino to send and recieve M-Bus packets to and from the
headunit, and based on commands from the headunit, control the iPod (over
its serial connection) appropriately.

And then document the crap out of it, because the internets are sorely
lacking in information on this.

## Index

- [The M-Bus Protocol](/mbus.md)
- [The Stock Civic Headunit](/radio.md)
- The iPod serial protocol (TODO)
- Putting it all together (TODO)
