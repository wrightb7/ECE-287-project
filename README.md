# ECE-287-project
Block Galaga in vhdl
as apart of our final project in ECE 287 we were asked to create a game using VHDL. 
This was a language we had very little experience with and from the start we were a bit overwhelmed.
The best start was to download the vga adapter from digikey @ https://www.digikey.com/eewiki/pages/viewpage.action?pageId=15925278
we started here and first getting an image to generate is a huge step. One thing i can say that took us a while to figure out 
was that you must set up the vga, imgae generator, and the altpll0 to work on the monitor that you are using. 
other than that google and trial and error were the best tools. we found a couple examples online we tried to mimic but the best
use of code we found second hand was the logic they used in making things work in vhdl.
Understading how to use the rising edge of the clock was the foundation we started on. That let us use what we knew about 
generating images and make them move. 
From there we started making great progress everytime we met. We set our game up with 4 "lanes" that objects spawned on and travled down
we added scoring for each block that travels all the way down. This was displayed on the 7segment led on our board. 
Hit detection was the next thing we tackled and the way we set up our logic for player position made it much more simple. we had several statements that said if a block is seen moving into the bottom most position and they player position 
