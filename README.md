# Website Performance Optimization portfolio project

## Part 1: Optimize PageSpeed Insights score for index.html

### Optimizations made:
* Minified style.css file, inlined, and moved to the header section
* Scripts were moved to the bottom of the body
* Loaded scripts asynchronously
* Removed link to Open Sans font

#### Instructions for testing:
* Copy and paste url: https://rld2121.github.io/websiteOpt into <a href = "https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Frld2121.github.io%2FwebsiteOpt">PageSpeed Insights</a>

#### Results on PageSpeed Insights
* Mobile -  91/100
* Desktop - 92/100


## Part 2: Optimize Frames per Second in pizza.html

### Optimizations made:
* Changed all instances of querySelector to getElementById and getElementsByClassName
* Under the changePizzaSizes function code, the following was done:
    * Moved document.getElementsByClassName out of the for loop
    * Cached the length used in the for loop
    * Deleted determineDx function and used the switch function to define newWidth
* Under the updatePositions function code, the following was done:
    * Moved document.getElementsByClassName out of the for loop
    * Cached the length used in the for loop
    * Cached the scrollTop request
    * Created a phase array 
* Under document.addEventListener fuction code, the following was done:
    * Defined elem outside the for loop
    * Moved document.getElementById out of the for loop
    * Changed amount of pizza loaded from 200 to 32
#### Instructions for testing:
* Load the <a href="https//rld2121.github.io/websiteOpt/views/pizza.html">Pizza site</a> and open Developer Tools.  With the console tab open, move the slider bar and scroll the page

#### Results
* Time to resize pizzas < 5ms
* Scroll Framerate = 60 fps
    
    

