# ng-decipher-intl-input
Angular Intenational telephone Input using jquery powered intl-input plugins

## What it does

### Initialization

`ngIntlTelInputProvider` is available to set configs in the module config phase.

### Validation

Operates as a normal validator for a form input based on the selected country.

### Formatting

Assigns the final formatted telephone number to the ng-model binding.

## Usage

### Installation

**Clone Git**

`git clone https://github.com/Prabakaran-t/ng-decipher-intl-input.git`

### Provider setup and config

Inject `ngIntlTelInput` into your application module

```javascript
var myApp = angular.module('myApp', ['ngIntlTelInput']);
```

### Directive usage

#### ng-intl-tel-input attribute

This attribute applies _intl-tel-input_ to a **text** or **tel** field.

```html
<input type="text" ng-model="model.tel" ng-intl-tel-input>
```

**Note**

* `type` is set to *text* or *tel*
* `ng-model` is specified (required)

| Method | Value | Description |
| --- | --- | --- |
| ng-intl-tel-input | - | This will initialize the intl-input plugins into the text box. |
| data-allowDropdown | true | false (by default true) | Enables Dropdown of flags container |
| data-autoHideDialCode | true | false (by default true) | if there is just a dial code in the input: remove it on blur, and re-add it on focus |
| data-customPlaceholder | string(Ex: Enter mobile no) | Your custom string for textbox placeholder |
| data-initialCountry | string(Ex: in) | country iso code to set the country as initial country |
| data-nationalMode | true | false (by default true) | if you don't want to insert international dial codes, set this method value as true |
| data-separateDialCode | true | false (by default true) | display the country dial code next to the selected flag so it's not part of the typed number |
| data-geoip | true | false (by default true) | Fetching user country using ipinfo.io and set country as initial country |
| data-onlyCountries | string(Ex: us,gb) | display only these countries, input must be Comma separated countries iso |


##Credits
* Intl Input[https://github.com/jackocnr/intl-tel-input]
* hodgepodgers[https://github.com/hodgepodgers/ng-intl-tel-input]