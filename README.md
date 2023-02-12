# AmazonFlexBot
Grab Amazon Flex offer with given price range
This program will work for Amazon Flex app that runs on "BlueStack5" android emulator.
To Set up and Run the program, You will need Windows machine since it's using windows
API for cliking actions, and Visual Studio with opencv installed. 

Next, You first need to train the model to learn the price numbers and symbols, 
TO DO so, Uncomment line 425 and Comment out line 427 to train model first. 
To train the model, you will want to screen capture some prices on Amazon Flex app, use it as
training input. NOTE: The size of your training has to match the size of your screen. For example, 
If you trained with image of a larger screen, but then run it on a smaller screen, the size different
may cause the model to read the price incorrect. so the size consistent is important.
When trainging start, simply type the number or character in the red box until it all finished.

Once Training is done, you can run Amazon Flex on android emulator BlueStack5 and run the program on visual studio, 
make sure there is nothing on top of your Flex app, otherwise, it won't be able to read the screen. 
Line 17 const int MIN_PRICE = 140; is where you can change the minimum price of offer you want to take, and 
Line 18 const float numBlocks = 0.4; is the height of screen you want to read, range from 0 to 1, the higher the value, 
the more blocks it can read. 
To Exit the program, simply type <strong>RIGHT CONTROL</strong> key, and the next you run the program, you will need to
press <strong>RIGHT CONTROL</strong> key again to activate the program. 

This is just a very simple version that does not offer much features. But hopefully it will help.

