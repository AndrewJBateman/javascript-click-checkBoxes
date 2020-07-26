# :zap: Javascript Click Checkboxes

Wes Bos Youtube Tutorial: [JS Checkbox Challenge! #JavaScript30 10/30](https://www.youtube.com/watch?v=RIPYsKx1iiU&list=PLu8EoSxDXHP6CGK4YVJhL_VWetA865GOH&index=11&t=0s).

*** Note: to open web links in a new window use: _ctrl+click on link_**

## :page_facing_up: Table of contents

* [General info](#general-info)
* [Screenshots](#screenshots)
* [Technologies](#technologies)
* [Setup](#setup)
* [Features](#features)
* [Status](#status)
* [Inspiration](#inspiration)
* [Contact](#contact)

## :books: General info

* Tutorial Code using javascript to select/deselect checkboxes.

## :camera: Screenshots

![Example screenshot](./img/check.png).

## :signal_strength: Technologies

* Ran in Google Chrome browser with: [Javascript engine V8 7.9.317.32 for Windows (x64)](https://v8.dev/).

## :floppy_disk: Setup

* Open index.html in browser. If any code is changed the browser needs to be refreshed.

## :computer: Code Examples

* Function to check 'in between' boxes if between selected boxes

```javascript
function handleCheck(e) {
  //check if they had the shift key down
  //AND check that they are checking it
  let inBetween = false;
  if (e.shiftKey && this.checked) {
    //loop over every single checkbox
    checkboxes.forEach(checkbox => {
      console.log(checkbox);
      if (checkbox === this || checkbox === lastChecked){
        inBetween = !inBetween;
        console.log('checking');
      }
      
      if (inBetween) {
        checkbox.checked = true;    
      }
    });
  }
```

## :cool: Features

*  Check boxes can be check/unchecked manually.

## :clipboard: Status & To-Do List

* Status: Working.
* To-Do: Nothing.

## :clap: Inspiration

* Wes Bos Youtube Tutorial: [JS Checkbox Challenge! #JavaScript30 10/30](https://www.youtube.com/watch?v=RIPYsKx1iiU&list=PLu8EoSxDXHP6CGK4YVJhL_VWetA865GOH&index=11&t=0s).

## :envelope: Contact

* Repo created by [ABateman](https://www.andrewbateman.org) - you are welcome to [send me a message](https://andrewbateman.org/contact)
