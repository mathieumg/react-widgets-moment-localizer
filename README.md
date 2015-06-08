
A date localization adapter for react-widgets using Momentjs. This _only_ handles date localization, if you plan on using the NumberPicker widget you will still need to include Globalize.js or some other number localizer.

    npm install react-widgets-moment-localizer

You can apply it by using the main module export, or the global object

```js
var widgets = require('react-widgets') // or window.ReactWidgets
  , moment require('moment')
  , momentLocalizer = require('react-widgets-moment-localizer')

widgets.configure.setDateLocalizer(momentLocalizer(moment));

//use the widgets

```

Or if you want to minimize the size of your build you can just require the confuration module

```js
var configure = require('react-widgets/lib/configure')
  , moment require('moment')
  , momentLocalizer = require('react-widgets-moment-localizer');

configure.setDateLocalizer(momentLocalizer(moment));

//use the widgets

```
