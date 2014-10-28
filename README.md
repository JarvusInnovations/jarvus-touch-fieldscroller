# jarvus-touch-fieldscroller
Monitors for field focus events and viewport resizes, ensuring that whatever scrollable container a field is within gets scrolled to make the focused field visible after a screen size change (or soft keyboard opening.)

## Installation
Just clone into your workspace's <kbd>packages</kbd> directory and add `"jarvus-touch-fieldscroller"` to the `"requires"` array of your Sencha Touch app's <kbd>app.json</kbd> file.

## Configuration
This override has one configuration option that can be set in your viewport configuration to adjust how many pixels of space it tries to create below the focused field. The padding should make it easy for the user to see and tap on the next field.

```js
Ext.application({
    name: 'MyTouchApp',

    viewport: {
        fieldFocusPadding: 10 // reduce focus padding from the default of 40
    }
    
    // ...
});
```
