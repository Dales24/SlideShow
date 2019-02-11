# SlideShow


This is a basic slide show created using javascript. 


I used a simple python server as a local host installed on my Mac. I used this because this is a very small project. I does need the massive additions that come with something like node js. I wanted something clean and easy to use.

Installing 
Open Terminal: 
Install Python if it is not already installed
brew install python
To connect to our server: 
python -m SimpleHTTPServer server 

We then access our local host and direct to where the Html and Image file are stored! 

You will need to modify the image source path based on where the image folder is saved.

ex:
/Desktop/slideshow/google.jpeg

Design and Dev: 

 I wanted to keep the code as simple as possible. My overall goal for the design was something functional, fast and reusable. It is important that the images are quicly loaded for a good user experience. 


I first create a div structure for each slide applying CSS classes for the text and images. I have a function currentSlide which keeps track of what slide you are on through indexing. I use this currentSlide function on my side nav bar. The side nav bar is originally hidden but can be opened and closed. I then move forward or backward by passing a -1 or 1 value to plusSlides. This is done when the back or next buttons are clicked. Next, I have a function showSlides which is looping through my array of slides. This functions hides all of my slides and sets the one that the user is on to visiable and there dot to active. 

To keep track of mobile swiping I have action eventlisteners for touching the screen. These event listeners then store the x and y coors of the touch into variables. This then allows me to determine wether the swipe came from the left or the right. 


Future Consideration: 

I would consider creating a json file in the future and looping through images. However, the current amount of data with these images is not very large. But, over time this area might want to be re-evaluated. I also considered loading images from a API, but this would also slow down the site. 
I would also like to improve the css style in the future. Style is always changing and can always be re-evaluted.
