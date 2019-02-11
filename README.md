# SlideShow


This is a basic slide show created using javascript. 


I used a Apache2 server as a local host already installed on my Mac.

Design: 

I first create a div structure for each slide applying CSS classes for the text and images. I have a function currentSlide which 
keeps track of what slide you are on through indexing. I use this currentSlide function on my side nav bar. The side nav bar is originally
hidden but can be opened and closed. I then move forward or backward by passing a -1 or 1 value to plusSlides. This 
is done when the back or next buttons are clicked. Next, I have a function showSlides which is looping through my array of slides.
This functions hides all of my slides and sets the ones that user are on to visiable and there dot to active. 

To keep track of mobile swiping I have action eventlisteners for touching the screen. These event listeners then store the x and y 
coors of the touch into variables. This then allows me to determine wether the swipe came from the left or the right. 

