## Website Performance Optimization portfolio project

### Usage

1. Clone this repository
`$ git clone https://github.com/Wapika/frontend-nanodegree-arcade-game.git`
2. Open index.html

#### OR

Visit the page hosted on Github -> [here] (https://wapika.github.io/)

### Optimizations

#### index.html
* Add `media=print` to the print.css link.
* Inline the CSS.
* Place the necessary CSS in the head, the rest at the end of the document.
* Remove the googleFont request.
* Load perfmatters.js and analytics.js asynchronously with `async`.
* Resize and optimize all the pictures.
* Minify and compress all the files.

#### pizza.html
##### slider
* Changes the slider value to a percent width.
* Store the selector in a variable outside the for loop.
* Iterates trough pizza elements and change their widths according to the value of the slider.
* Change the width style directly instead of calculating an offset width.

##### background pizzas
* Store the scrollTop value outside the for loop.
* Iterate over the pizzas and apply the new style. I tried with `transform : translateX` but the results were almost identical.
* Use the RAF method for rate-limiting the execution of the function.
* Reduce the number of pizzas from 200 to 30.
