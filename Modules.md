## NPM. Modules

* [Presentation](https://slides.com/danielsuleiman/npm#/)	
* Install [browserify](http://browserify.org/)	
* Install [babelify](https://github.com/babel/babelify)
* Implement Counter based on modules	
  * Create folder **modules** and **idnex.js** inside	
  * Create module **Counter.js** (class with state, and methods for increment / decrement)
  * Create module **Element.js**. Class wich should work like:
```	  * Create **src** folder

// Element.js

class Element {
    constructor(elem) {
       
    }

    addClassName(className) {
     
    }

    onClick(callback) {
       
    }

    update(children = []) {

    }

    render(children = []) {
       
    }    
}


// decrementButton.js

import { Element } from './Element'

 export const decrementButton = new Element('div')
.addClassName('button')
.addClassName('center')
.addClassName('decrement')


// index.js

import { decrementButton, incrementButton, counterBlock, wrapper, container, Counter }  from './modules'


const counter = new Counter()

counter.onChange(currentValue => {
 counterBlock.update([currentValue])



document.body.append(
     wrapper.render([
        counterBlock.render([counter.currentValue]),
        container.render([
            leftButton.onClick(counter.dicrement).render(['-']),
            resetButton.onClick(counter.reset).render(['#']),
            rightButton.onClick(counter.increment).render(['+'])
        ])
    ])
 )
})
```	

* Everything should work without any html tags inside.	
<img src="./assets/counter.png" width="400">

* styles you can find [here](https://github.com/tr3v3r/simple-counter/blob/master/styles.css) 
  
## Hometaks
Rewrite your **weather-app** using modules.

Your app should consist of at least several modules. i.e.
* Module for fetching data
* Module for rendering and manging map
* Module for rendering and mangin table
* Module for handling localstorage
* Module createElement 


