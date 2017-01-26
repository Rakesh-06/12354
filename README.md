# Website Performance Optimization portfolio project



### INTRO

	Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! 
In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

To get started, check out the repository and inspect the code.


### Getting started

##### Part 1: Optimize PageSpeed Insights score for index.html

##### Part 2: Optimize Frames per Second in pizza.html

				To optimize views/pizza.html, you will need to modify views/js/main.js until your frames per second rate is 60 fps or higher. 
You will find instructive comments in main.js. 

You might find the FPS Counter/HUD Display useful in Chrome developer tools described here: [Chrome Dev Tools tips-and-tricks](https://developer.chrome.com/devtools/docs/tips-and-tricks).


#### To get Started

	Follow the github link to get into the optimized website repo https://rakesh-06.github.io/12354/. Clone it or download as zip to the local system. Open index.html and pizza.html in your browser and use devtools.
	

### Solution

* All images are made available loally in the respective img folders. 
	-The images were made to reduce in size by using effective online compressor software [optimizilla](www.optimizilla.com).

* The CSS files were minified using online minifier.
	- Thses files were inlined with the index.html. (added at the end of the body).
	- Print attribute was added to print.css to avoid blocking of CRP and moved to end of HTML body.

* prefmatters.js given with async to avoid CRP blocking. Script files were also minified online.

* pizza.html was made to scroll at 60fps and optimized. 

* Eliminated DetermineDX function to avoid complexity.

* Width of Pizza expressed as percentage.

* querSelectors were plaed outside the loops to avoid FSL issues and complexity.

* PageSpeed Insights Score (image form) included with the source file.

* var were defined out of the loop at some places (elem, phase).

**Changes made as per reviewer suggestion**

	* Changed the querySelectors with getElementById and getElementsByClassName
	
	* changePizzasize function is eliminated and the width modification were placed inside changeSliderLabel Function itself.
	
	* The number of pizzas covering the user screen was calculated based on user's screen.

##### PAGESPEED INSIGHTS SCORE

https://developers.google.com/speed/pagespeed/insights/

* mobile: 93 / 100

* desktop: 96 / 100



##### Optimized website source code available at : https://rakesh-06.github.io/12354/

	
	

