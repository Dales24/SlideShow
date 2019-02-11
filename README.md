# SlideShow


This is a basic slide show created using javascript. 


I used a simple python server as a local host installed on my Mac. I used this because this is a very small project. I dont need the massive additions that come with something like node js. I wanted something clean and easy to use.

# Installing 
Open Terminal: 
Install Python 2.7 if it is not already installed

To connect to our server: 
`python -m SimpleHTTPServer`

Go to localhost:8000/slideshow.html 


# Design and Dev: 

 I wanted to keep the code as simple as possible. My overall goal for the design was something functional, fast and reusable. It is important that the images are quicly loaded for a good user experience. 


I first create a div structure for each slide applying CSS classes for the text and images. I have a function currentSlide which keeps track of what slide you are on through indexing. I use this currentSlide function on my side nav bar. The side nav bar is originally hidden but can be opened and closed. I then move forward or backward by passing a -1 or 1 value to plusSlides. This is done when the back or next buttons are clicked. Next, I have a function showSlides which is looping through my array of slides. This functions hides all of my slides and sets the slide that the user is on to visible.

To keep track of mobile swiping I have action eventlisteners for touching the screen. These event listeners then store the x and y coordinate of the touch into variables. This then allows me to determine if the swipe came from the left or the right. 


# Future Consideration: 

I would consider creating a json file in the future and looping through images. However, the current amount of data with these images is not very large. But, over time this area might want to be re-evaluated. I also considered loading images from a API, but this would also slow down the site. 
I would also like to improve the css style in the future. Style is always changing and can always be re-evaluated.
