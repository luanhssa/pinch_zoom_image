# Pinch Zoom Image

A widget that makes picture pinch zoom, Instagram style!

![](https://i.imgur.com/AkKX9qZ.gif)

## Installation

Add this to your `pubspec.yml` dependencies:

```
pinch_zoom_image: "^0.0.2"
```

## How to use

Add the widget to your app like this (It automatically takes the size of the image you pass to it):

```dart
PinchZoomImage(
  image: Image.network('https://i.imgur.com/tKg0XEb.jpg'),
  zoomedBackgroundColor: Color.fromRGBO(240, 240, 240, 1.0),
),
```

The `zoomedBackgroundColor` is the color that fills the image's space when the use is zooming it and moving it on the screen.

If you want images from internet to be cached for offline use or data saving, you can also use this with the [cached_network_image widget](https://pub.dartlang.org/packages/cached_network_image):

```dart
PinchZoomImage(
  image: Image(
    image: CachedNetworkImageProvider('https://i.imgur.com/tKg0XEb.jpg'),
  ),
  zoomedBackgroundColor: Color.fromRGBO(240, 240, 240, 1.0),
),
```

Enjoy!