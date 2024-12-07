this started cause i wanted to make a ball move around the screen based on me moving the m5stickcplus. 
then i realized it could make a good way to navigate the stick.
one limitation of the stick is its lack of user interface options 3 buttons. one for power.
still working on this and will just keep any projectors that fit here while i keep fooling around.
it uses the 6 Axis IMU. 3 Axis Gyroscope. 3 Axis Acceloremeter.

first i started with: 
ballmove: the ball moves and rolls around the screen

then:
ballbounce: the ball has some bounce when it hits the walls and build momentum

then:
infiniteball: the ball really quickly gains momentum and  into ∞ symbol

then:
menunavigationv1: the first iteration. really flickable

then:
menunavflick: more directional. menu goes next and back

then:
menunavtap: gets acceleration data. over 2.00 registers menu - next

  *CHANGE -const float movementThreshold = 1.50; // Threshold for ax, ay, az to trigger menu change
        if you want to make it more or less sensitive change value. 2 is most stable. less unitentional movement. 1 very responsieve. quick flicks. will probably replace flick navigation with this and just change value... 1.5 is a nice medium

        M5.Lcd.setRotation(1); change (1) to 1-4 to set screen rotation
