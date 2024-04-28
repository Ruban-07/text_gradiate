# Text Gradiate 👉🏻 For Colorful Texts

![Version Badge](https://img.shields.io/pub/v/text_gradiate?color=green)
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
[![GitHub repo](https://img.shields.io/badge/GitHub-purple?logo=github)](https://github.com/Ruban-07/text_gradiate)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/ruban-raghavendar-k/)
[![Gmail](https://img.shields.io/badge/Gmail-Send%20Email-red?style=flat-square&logo=gmail)](mailto:rubanraghavendar@gmail.com)

[![Android](https://img.shields.io/badge/Android-Supported-brightgreen)](https://developer.android.com/)
[![iOS](https://img.shields.io/badge/iOS-Supported-brightgreen)](https://developer.apple.com/ios/)

A Flutter package for creating gradient text in an fastest way. This package allows you to add gradient effected text in your Flutter app effortlessly.

## Features🌈

- Easily create text with gradient colors.
- Customize gradient colors and types, including linear, radial, or sweep gradients.
- Control various gradient properties such as starting and ending points, tiling strategy, center and focal points, focal radius, angles, stops, and transform matrix.

## Screenshots📸

<div>
  <img src="https://ruban-07.github.io/text_gradiate/assets/images/samp1.jpg" width="300" alt="sample-image 1" />
  <img src="https://ruban-07.github.io/text_gradiate/assets/images/samp2.jpg" width="300" alt="sample-image 2" />
  <img src="https://ruban-07.github.io/text_gradiate/assets/images/samp3.jpg" width="300" alt="sample-image 3" />
</div>

## Installation📦

To use this package, add `text_gradiate` as a dependency in your `pubspec.yaml` file.

```yaml
dependencies:
  text_gradiate: ^1.0.0
```

Then, import the package into your Dart code:

```dart
import 'package:text_gradiate/text_gradiate.dart';
```

## Usage🛠️

Wrap your text widget with `TextGradiate` and specify the desired gradient properties.

```dart
TextGradiate(
  text: Text(
    'Hello, Gradient!',
    style: TextStyle(fontSize: 24.0),
  ),
  colors: [Colors.blue, Colors.green],
  gradientType: GradientType.linear,
  begin: Alignment.centerLeft,
  end: Alignment.centerRight,
  tileMode: TileMode.clamp,
)
```

## Example🫣

Here's a simple example that shows how to use the `TextGradiate` widget with some properties:

```dart
import 'package:flutter/material.dart';
import 'package:text_gradiate/text_gradiate.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('TextGradiate Example'),
        ),
        body: Center(
          child: TextGradiate(
            text: Text(
              'Hello, Gradient!',
              style: TextStyle(fontSize: 24.0),
            ),
            colors: [Colors.blue, Colors.green],
            gradientType: GradientType.linear,
            begin: Alignment.centerLeft,
            end: Alignment.centerRight,
            tileMode: TileMode.clamp,
          ),
        ),
      ),
    );
  }
}
```

## Properties Usage🫧

- `text`: The child widget to which the gradient effect will be applied.

- `colors`: The list of colors to use for the gradient.

- `gradientType`: Specifies the type of gradient (`linear`, `radial`, or `sweep`).

- `begin` (for linear gradients): The starting point of the gradient.

- `end` (for linear gradients): The ending point of the gradient.

- `tileMode` (for linear gradients): The tiling strategy for the gradient.

- `center` (for radial and sweep gradients): The center point of the gradient.

- `focal` (for radial gradients): The focal point of the gradient.

- `focalRadius` (for radial gradients): The focal radius of the gradient.

- `startAngle` (for sweep gradients): The starting angle of the gradient.

- `endAngle` (for sweep gradients): The ending angle of the gradient.

- `stops`: The stops of the gradient.

- `transform`: The transform matrix for the gradient (applicable only for linear and sweep gradients).

```dart
TextGradiate(
  text: Text(
    'Hello, Gradient!',
    style: TextStyle(fontSize: 24.0),
  ),
  colors: [Colors.blue, Colors.green],
  gradientType: GradientType.linear,
  begin: Alignment.centerLeft,
  end: Alignment.centerRight,
  tileMode: TileMode.clamp,
)
```

## Support❤️

- Android: Supported on SDK 16 and above.
- iOS: Supported on iOS 11.0 and above.
- Linux: Any Linux distribution.
- macOS: Supported on macOS 10.14 and above.
- Web: Supported on all web browsers.
- Windows: Supported on all Windows versions.

---
