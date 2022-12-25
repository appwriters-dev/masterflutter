---
id: ls05-button-layout
title: Button Layout
---


A button is made up of an icon or text (or both). When the user touches it, the click event is triggered and the appropriate action is taken. Flutter has a variety of buttons. These button types are used for a variety of purposes. This story will teach you how to use them for your own benefit.

## Projects

### 1. Flat Button

Create a flat button with a simple text. with the two properties `child` and `onPressed ()`. Then you can use its attributes to decorate it (`colour, text size etc.`).

### 2. Raised Button

Create a raised button with a simple text `Raised Button`. with the two properties `child` and `onPressed ()`.

```dart
/// Try this code example on your device 
RaisedButton(
          onPressed: () => {
            Print("Pressed");
},
          child: Text('Raised Button'),
        ),
```

### 3. Text Button

Create a Text button with a simple text `Text Button`. with the properties `child` and `onPressed ()`,`onLongPress ()`.


```dart
 TextButton(
     child: Text('Text Button'),
     onPressed: () {
         print('Pressed');
      },
   onLongPress: () { 
       print('Long press');
},
)
```
### 4. Icon Button

Make an IconButton with the Material icon "volume up" and text.

### Make the UI , publish it on your github, and share it on social media.

![Button layout](/images/ch05-ls05-btn-01.png)


## Resources

- [Flutter Layout Widgets](https://flutter.dev/docs/development/ui/layout)
- [Examples of Button and Style](https://androidride.com/flutter-raisedbutton-examples)
- [Flat Button](https://www.tutorialkart.com/flutter/flutter-flatbutton)
- [Floating Button](https://api.flutter.dev/flutter/material/FloatingActionButton-class.html)
- [Text Button](https://api.flutter.dev/flutter/material/TextButton-class.html)
- [Text Button](https://www.woolha.com/tutorials/flutter-using-textbutton-widget-examples)
- [Text Icon Button](https://www.woolha.com/tutorials/flutter-using-textbutton-widget-examples)
- [Icon Button](https://api.flutter.dev/flutter/material/IconButton-class.html)
