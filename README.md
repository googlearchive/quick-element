## Quick Element

When you are writing a demo or a test for your Polymer app or component, it is
sometimes nice to be able to add an element inline with the tests or demo
implementation. Quick Element is a custom element that will help you to do this
without resorting to using an HTML Import.

### Usage

```html
<!-- Declare an element called "x-greeter" -->
<template is="quick-element" name="x-greeter">
  <h1><span>{{greeting}}</span>, <content></content></h1>
</template>

<!-- Use "x-greeter" elsewhere in the document -->
<x-greeter greeting="Hello">World</x-greeter>
<x-greeter greeting="Live long and prosper">Dumbledore</x-greeter>
```
