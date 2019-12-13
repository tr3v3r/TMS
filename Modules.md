## NPM. Modules

* [Presentation](https://slides.com/danielsuleiman/npm#/)
* Install [browserify](http://browserify.org/)
* Install [babelify](https://github.com/babel/babelify)
* Implement Counter based on modules
  * Create folder **modules** and **idnex.js** inside
  * Create module **Counter.js** (class with state, and methods for increment / decrement)
  * Create module **createElement.js**. Function wich should work like:
```
 const decrementButton = createElement(
   'div',
   { style: "button center decrement", onClick: () => { // your code on click } },
   [
     "-"
   ]

 <div style="button center decrement">"-"</div>
```
* Re export this modules to make possible use them like `import { Counter, createElement } from './modules'`
* Create **index.js** near **modules** folder and using *Counter* and *createElement* create 3 buttons and counter element
* Everything should work without any html tags inside.


  
