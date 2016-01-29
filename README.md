# ko-forcedFormat
Forces the format of an observable to be to a pattern
(The knockout version of https://github.com/firstopinion/formatter.js)

## Usage
```javascript
function ViewModel(){
      var self = this;
      self.value = ko.observable().extend({forceFormat: '(###)-###-####'});
    }
  ko.applyBindings(new ViewModel());
```

```html
<input type="text" data-bind="textInput: value">
```

This will format any characters entered into the input to phone format
