## ES6. Destructuring. Functions.

* [Presentation](https://slides.com/danielsuleiman/es6#/)


## Hometask
* Downdload [this](https://github.com/tr3v3r/destructuring)
* Clone your **TMS-your-name** repository
* Copy downloaded folder into you project
* Commit changes and push into master of your TMS-your name repository

* Create and switch to branch with name **desctructuring**
* Create folder with name **desctructuring**
* Open **desctructuring** folder in your VSCode / WebStorm
* `npm install`
* Open **test** folder and fix all tests
* Run `npm run test ./test/file name.js` to check. ( i.e. for **string.js** `npm run test ./test/string.js` )
* Push branch and open Pull Request

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
