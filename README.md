##Website Optimization
In this project, I optimized the Critical Rendering Path in index.html until it achieved a score of at least 90 on desktop & mobile using Google's PageSpeed Insights tool [](https://developers.google.com/speed/pagespeed/insights/)

I also made optimizations to views/js/main.js to make views/pizza.html render consistently at 60fps while scrolling

Lastly, I optimized the pizza resize slider so that time to resize is under 5ms

To open the project, open index.html in the browser. Click on the "Cam's Pizzeria" link to view the optimizations there

###index.html
<ul>
  <li>Minified html</li>
  <li>Implemented media="print"</li>
  <li>Resized large images</li>
</ul>

###views/js/main.js
<ul>
  <li>Refactored "document.querySeclector" calls to faster "document.getElementById"</li>
  <li>Reduced number of sliding pizzas in DOMContentLoaded listener</li>
  <li>Removed forced synchronous layout from updatePositions function</li>
  <li>Use transform CSS property and translateX to animate sliding pizzas in updatePositions function</li>
  <li>Removed forced synchronous layout from changePizzaSizes function</li>
  <li>Added requestAnimationFrame to both functions</li>
</ul>
