## DOM. BOM

* [Presentation](https://slides.com/danielsuleiman/dombom/#/)
* Notifications
  * Clone [this](https://github.com/tr3v3r/notification) repository
  * Notification must be shown after page loads and hide after 5 seconds.
  * Closing icon. Click on it closes the component
  * Checkbox that disables notification and sets a flag into local storage. If the flag is set, component won't be shown when the page reloads
  * Add logic for arrows ( left/ right ). Change notification text and active dot.
  * Keyboard support. Component supports keyboard control: switching back and forward, closing by clicking on the cross.

<img src="./assets/notification.png" width="400">

## Hometask ( Upgrade you weather-app)
### To do this task please complete class fork from [previous classes](https://github.com/tr3v3r/TMS/blob/master/Async.md)
* Clone your **TMS-your-name** repository
* Create and switch to branch with name **weather-app-bom**
* Add a My weather button, clicking it wil interact with **navigator.geolocation** API and fetch weather data of your current location;
* Store fetched data at the localstorage and render it in the a table;
* Update your data from a localstorage with the newest from the server when access the app; ( When open page you shuld take all saved cities and re-fetch data )
* After competing the task maket pull request for review
