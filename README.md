# DEPRICATED
Please see ko-formatter for newer version

## ko-forcedFormat


ko-forcedFormat is a simple knockout js extender that originated from firstopinion's javascript plugin (found here:  https://github.com/firstopinion/formatter.js)

## Usage

Working example in the src folder
```javascript
function ViewModel(){
      var self = this;
      self.value = ko.observable().extend({forceFormat: '(###)-###-####'});
    }
  ko.applyBindings(new ViewModel());
```

```html
<!--Use the textInput binding for format at key press -->
<input type="text" data-bind="textInput: value"> 
```

This will format any characters entered into the input to phone format
