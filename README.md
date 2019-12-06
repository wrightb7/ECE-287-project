# ECE-287-project
Block Galaga in vhdl
as apart of our final project in ECE 287 we were asked to create a game using VHDL. 
This was a language we had very little experience with and from the start we were a bit overwhelmed.
The best start was to download the vga adapter from digikey @ https://www.digikey.com/eewiki/pages/viewpage.action?pageId=15925278
we started here and first getting an image to generate is a huge step. One thing i can say that took us a while to figure out 
was that you must set up the vga, imgae generator, and the altpll0 to work on the monitor that you are using. 
other than that google and trial and error were the best tools. we found a couple examples online we tried to mimic but the best
use of code we found second hand was the logic they used in making things work in vhdl.

Understading how to use the rising edge of the clock was the foundation we started on. That let us use, what we knew about 
generating images and make them move. 
From there we started making great progress everytime we met. We set our game up with 4 "lanes" that objects spawned on and travled down
we added scoring for each block that travels all the way down. This was displayed on the 7 segment led display on our board. 
Hit detection was the next thing we tackled and the way we set up our logic for player position made it much more simple. we had several 
statements that said if a block is seen moving into the bottom most position and they player position is in that lane subtract one life. 
so 3 lives = binary "11", 2 lives "10", and 1 life "01" so we stop the game when that last life is taken away. We displyed that on our
board aswell with 3 green leds.

After we reached that point we felt like the base game was in a good spot. We did decide to take on a couple challanges to make the game 
stand out and try to experiment with what we had learned. Using a second variable and attaching it to another clock speed to generate more
images that fall at greater speeds and used these two spawn rates to make something that would resemble levels. We set the one clock speed
to trigger when the game starts. Then after you reach a certian score switch to the faster clock speed. Lastly once another higher score 
was reached run them both at the same time. 

The last thing we decided to put in was a spur of the moment idea the save the most recent score and display it next to the current score.
this was fairly simple but did take sometime to get working. The idea was to say once the reset button was pressed take the binary values 
stored in the first set and move them over and bring then initial values back to zero.

The game was an equal amount of challenging and fun, it gave us a glimpse of what its like to program in VHDL. This whole process has done a lot to improve my critical thinking and the way I approch new problems. There were some other things i would have liked to try to do with the game but in the amount of time we had i am very proud of what we got done and how much we learned.
