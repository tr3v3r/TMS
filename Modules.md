## NPM. Modules

* [Presentation](https://slides.com/danielsuleiman/npm#/)	* [Presentation](https://slides.com/danielsuleiman/webpack/#/)
* Install [browserify](http://browserify.org/)	* **npm i --save-dev webpack**
* Install [babelify](https://github.com/babel/babelify)	* **npm i --save-dev webpack-cli**
* Implement Counter based on modules	* **npm i --save-dev style-loader**
  * Create folder **modules** and **idnex.js** inside	* **npm i --save-dev css-loader**
  * Create module **Counter.js** (class with state, and methods for increment / decrement)	* create **webpack.config.js** and set up config (*style-loader*, *css-loader* with modules support, *html-webpack-plugin*)
  * Create module **createElement.js**. Function wich should work like:	* Implement Search/Add. 
```	  * Create **src** folder
 const decrementButton = createElement(	  * Try to split your logic into modules ( i.e. Form, Box, Store ) 
   'div',	
   { style: "button center decrement", onClick: () => { // your code on click } },	
   [	
     "-"	
   ]	


 <div style="button center decrement">"-"</div>	<img src="./assets/search.png" width="600">
```	

* Re export this modules to make possible use them like `import { Counter, createElement } from './modules'`	
* Create **index.js** near **modules** folder and using *Counter* and *createElement* create 3 buttons and counter element	
* Everything should work without any html tags inside.	
<img src="./assets/counter.png" width="400">

  
## Hometaks
Rewrite your **weather-app** using modules.

Your app should consist of at least several modules. i.e.
* Module for fetching data
* Module for rendering and manging map
* Module for rendering and mangin table
* Module for handling localstorage
* Module createElement 


