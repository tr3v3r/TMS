## ES6 Strings. Iterators. Generators. Map, Set

* [Presentation](https://slides.com/danielsuleiman/es6#/3)



## Hometask
* Downdload [this](https://github.com/tr3v3r/es6-features-practise)
* Clone your **TMS-your-name** repository
* Create folder with name **es6-features-practise** in master branch
* Copy files from repository from *step 1* to **es6-features-practise** folder
* push your changes into master
* Create and switch to branch with name **es6-features-practise**
* Open **es6-features-practise** folder in your VSCode / WebStorm
* `npm install`
* Open **test** folder and fix all tests
* Run `npm run test ./test/file name.js` to check. ( i.e. for **symbol.js** `npm run test ./test/symbol.js` )
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
