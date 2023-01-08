---
id: ls01-images
title: Images
---

Images are a common type of asset in mobile applications. We will learn how to include images in our application and use them in the user interface.

## Projects

### 1. Your Business Card

Create a UI that displays your business card along with your photo. Your photo should be kept inside `assets/images` folder. You can use any image you like.

> **Note:** Use `Image.asset` to load the image from assets. Check [pubspec assets](https://flutter.dev/docs/development/ui/assets-and-images#declaring-assets) for more information.

### 2. Dice Roller

Refactor dice app from previous chapter to use the image of Dice instead of the number.

> **Note:** It's a good practice to keep all the asset names as a constant by creating a class. This will help you to avoid typos and make it easier to change the asset name in the future.

For example:
    
```dart
    class Assets {
      static const String dice1 = 'assets/images/dice1.png';
      static const String dice2 = 'assets/images/dice2.png';
      static const String dice3 = 'assets/images/dice3.png';
      static const String dice4 = 'assets/images/dice4.png';
      static const String dice5 = 'assets/images/dice5.png';
      static const String dice6 = 'assets/images/dice6.png';
    }
```

## Resources

- [Image Widget](https://api.flutter.dev/flutter/widgets/Image-class.html)
- [Image.asset](https://api.flutter.dev/flutter/widgets/Image/Image.asset.html)
- [Pubspec assets](https://flutter.dev/docs/development/ui/assets-and-images#declaring-assets)