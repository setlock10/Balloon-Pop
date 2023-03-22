This is not your father’s balloon pop game

This one leverages the front facing camera and the handtrackjs library to recognize gestures and pop balloons without ever touching the screen. 

The genesis of this project was the thought I had that the front facing cameras on all of our computers, phones and tablets were being underutilized as an input device and that if used properly could address some accessibility issues. 

Starting simple I thought of Balloon Pop without having to touch the screen. 


My first attempt to solve the problem started with simple  motion detection.  Where motion detection is achieved by comparing the most recent frame of video with the previous frame of video.  


This method of detecting motion is great for things like home security or pet cams and could be used to create alerts automatically when the video feed is displaying something new.  

But it was not the solution I needed. I needed to be able recognize my tapping gesture and identify where on the screen I was tapping.  


I eventually found handtrackjs created by victor dibia. Handtrackjs is a library that performs realtime hand detection directly in the browser.   

Handtrackjs returns a probability of the presence of different objects like open hand, closed hand, pinch and point as well as face detection.   And can detect up to 100 instances in each image by using an object detection neural network model that has been trained using the tensorflow object detection api.   

Once I had set up handtrackjs and got it to the point where it would place a reticle on the screen at the tip of my finger there was just the minor step left of creating the ballon pop portion of the project. 

It was just a simple matter of painting some balloons, creating a balloon pop animation, animating the balloon movement, handling the collision detection, creating sound effects and then coding it all up in javascript.  

This was a very rewarding project and I am grateful for the libraries people have created that we can use to create new things.  