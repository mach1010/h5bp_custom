### HTML5 Boilerplate with Bourbon, Neat, and Bitters
A basic template based on [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate) augmented with the [Bourbon CSS Library](http://bourbon.io/) family (Neat/Bitters/Refills).  

HTML5 is a great base template and can be easily customized at [Initializr](http://www.initializr.com/) for several types of projects. It offers a responsive framework which is not included in this repo since Neat is also a responsive grid system.

#### NOTES
CSS goes in `public/assets/css` if you want to add vanilla css.  
If you want to use SASS (.scss actually) then add your css rules to partials in the scss/ directory...  

scss/  
|-- **base** contains the Bitters mixins. Add/change variables, typography, forms, etc. in here  
|  
|-- **partials** add `_partial.scss` files in here to add and organize your css rules
|  
|-- **vendor** contains bourbon and neat mixins and normalize
|
|-- **main.scss** add your partials here so they get processed. example: `@import partials/partial`  

Then from the base directory, run `sass --sourcemap=none --watch --scss scss:public/assets/css` to process scss as you work.  