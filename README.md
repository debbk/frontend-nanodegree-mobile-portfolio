## Website Performance Optimization portfolio project
[View Project](http://debbk.github.io/frontend-nanodegree-mobile-portfolio)

###Setup and Testing the Page Speed
1. Clone the repository to local machine
2. Start XAMPP server ([instructions on XAMPP installation](https://www.apachefriends.org/index.html))
3. Open a browser and visit the local host (ex. http://localhost:8080/udacity/p4)
4. Download [ngrok](https://ngrok.com/) and run it from the command line to make the local server accessible remotely
5. Copy the URL output via ngrok and run it through [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)



####Part 1: Optimize PageSpeed Insights score for index.html

Index.hmtl was optimized with the following:
1. Inlined style.css
2. Utilized grunt to minimize images
3. Removed webfont
4. Added async to non-render blocking js
5. Included media print in call to print.css
6. Minified CSS and JS


####Part 2: Optimize Frames per Second in pizza.html

Views/pizza.html was optimized with the following:
1. Put class 'mover' on a separate layer
2. Reduced the number of pizzas generated from 200 to 25
3. Moved the calculation of 'document.body.scrollTop / 1250' outside of the loop on line 493
4. Changed the 'changePizzaSizes' function so the size of the pizza is calculated immediately (without the need of the dx function)
5. Utilized grunt to minimize images
6. Added meta tags
7. Inlined style.css
8. Minified CSS and JS
