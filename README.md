## Website Performance Optimization portfolio project

This goal of this project is to optimize and enhance the performance of website.


### Getting started
Check out [Udacity Repository](https://github.com/udacity/frontend-nanodegree-mobile-portfolio "Udacity web performance") and download the code. To run it:
1. Download and install npm from this [link](https://www.npmjs.com/ "npm")
1. Open cmd and run this command: `npm install http-server -g`
1. Run your website on http-server with this command: `http-server [PATH]` Path to your project location. 
1. Open a browser and open your website through: `localhost:8080`
1. To check your local host website speed score by Google PageSpeed, run remote server with the follwoing steps: 
	* Download and install ngrok from this [link](https://ngrok.com "ngrok"), unzip it and run it.
	* To create remote server URL, type this command: `ngrok.exe http 8080`
	* Copy the created link and paste it in PageSpeed Insight.


### Part 1: Optimize PageSpeed Insights score for index.html
* Optimize images provided by Google's PageSpeed Insight
* Elemenate redner-blocking JS and CSS:
	* Google analytics JS using `async`
	* Add media query `print` for print.css
	* Using Web Font Loader to render Google Fonts api
* Minify and compressed Index.html, style.css

### Part 2: Optimize Frames per Second in pizza.html
The main optimization in main.js are getting variables creation and calcultioins out of the loop, dynamically getting the backgournd pizzas number based on screen height and replacing `.querySelector()` by `.getElementByClassName()`.