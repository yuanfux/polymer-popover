# \<classic-popover\>
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/yuanfux/classic-popover)

A Polymer popover component empowered by Popper.js

## Preview
An easy to use and run-time configurable popover component based on Polymer 2.0.

![gif broken](https://drive.google.com/uc?id=119jxrSGKR4FqHORDuBFiri3W4qDIV1Nx "classic-popover-demo")

## Install
1. Install bower dependency

   `bower install classic-popover --save`

2. Import classic-popover component into your project

   `<link rel="import" href="YOUR_PATH/bower_components/classic-popover/classic-popover.html"`

## Usage
### Quick Start
Specify `for`, `placement`, `content` and make sure your target element is inside `body` tag of the document. For more examples, please check out the demo in the `demo` folder.
<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="classic-popover.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<div style="overflow: scroll; width: 2000px; padding: 350px;">
	<div id="target" style="display: block; width: 50px; height: 50px; background-color: pink">
	</div>
</div>
<classic-popover for="target" placement="left" content="This is the popover content">
</classic-popover>
```

## Properties

Prop Name | Description | Type | Example | Default | Reactive
--- | --- | --- | --- | --- | ---
for | the attached target element id | string | 'reference' | - | true
placement | the initial placement of popover | string | 'top', 'right', 'bottom', 'left' | 'bottom' | true
content | the content of popover | string | 'popover content' | - | true
header | the header of popover | string | 'popover header' | - | true
offset | the offset of popover | string | '10, 10', '10%, 10', '10%, 10%' | '0, 0' | true
z-index | the z-index of popover | number | 1000 | 999 | true
type | the type of popover header | string | 'default', 'danger', 'warning', 'info', 'success', 'primary' | true
custom | if true the `content` will be omitted, `slot` will be enabled | boolean | false | false | false
hidden | if true the popover will be visible | boolean | false | false | true

## Slots

Slot Name | Description
--- | --- 
custom-content |  customized html content when `custom` is true  

## License
MIT
