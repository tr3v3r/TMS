## ES6. Destructuring. Functions.

* [Presentation](https://slides.com/danielsuleiman/es6#/)


## Hometask
* Fork [this](https://github.com/tr3v3r/destructuring/blob/master/README.md)
* In *TMS-your name* add link to this repository in README.md
* Add **tr3v3r** as collaborator
* Clone repository
* `npm install`
* Open **test** folder and fix all tests
* Run `npm run test ./test/file name.js` to check. ( i.e. for **string.js** `npm run test ./test/string.js` )

### Example
* Open file **test/array.js**
* take first task
```
 it('extract value from array, e.g. extract 0 into x like so `let [x] = [0];`', () => {
      let firstValue = [1];
      assert.strictEqual(firstValue, 1);
 });
```
* Change code inside **it** to pass test
```
 it('extract value from array, e.g. extract 0 into x like so `let [x] = [0];`', () => {
      let [firstValue] = [1];
      assert.strictEqual(firstValue, 1);
 });
```
* `npm run test ./test/array.js`
