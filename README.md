## Website Performance Optimization portfolio project

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
