---
id: ls05-button-layout
title: Button Layout
---


A button is made up of an icon or text (or both). When the user touches it, the click event is triggered and the appropriate action is taken. Flutter has a variety of buttons. These button types are used for a variety of purposes. This story will teach you how to use them for your own benefit.

## Projects

### 1. Button Layout

Create buttons with a text and icons. with the two properties `child` and `onPressed ()`. Then you can use its attributes to decorate it (`colour, text size etc.`).

![Button layout](/images/ch05-ls05-btn-01.png)

> Note: Make sure to explore different properties of `button` widget you used . For example, you can see two type of button sample code .

```dart
/// Try this code example on your device 
RaisedButton(
          onPressed: () => {
            Print("Pressed");
},
          child: Text('Raised Button'),
        ),
```

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


## Resources

- [Flutter Layout Widgets](https://flutter.dev/docs/development/ui/layout)
- [Examples of Button and Style](https://androidride.com/flutter-raisedbutton-examples)
- [Flat Button](https://www.tutorialkart.com/flutter/flutter-flatbutton)
- [Floating Button](https://api.flutter.dev/flutter/material/FloatingActionButton-class.html)
- [Text Button](https://api.flutter.dev/flutter/material/TextButton-class.html)
- [Text Button](https://www.woolha.com/tutorials/flutter-using-textbutton-widget-examples)
- [Text Icon Button](https://www.woolha.com/tutorials/flutter-using-textbutton-widget-examples)
- [Icon Button](https://api.flutter.dev/flutter/material/IconButton-class.html)
