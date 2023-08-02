# Flutter_doc_CokBK_GES_Add_Material_touch_ripples
 https://docs.flutter.dev/cookbook/gestures/ripples
Add Material touch ripples
==========================

1.  [Cookbook](https://docs.flutter.dev/cookbook)
2.  [Gestures](https://docs.flutter.dev/cookbook/gestures)
3.  [Add Material touch ripples](https://docs.flutter.dev/cookbook/gestures/ripples)

Widgets that follow the Material Design guidelines display a ripple animation when tapped.

Flutter provides the [`InkWell`](https://api.flutter.dev/flutter/material/InkWell-class.html) widget to perform this effect. Create a ripple effect using the following steps:

1.  Create a widget that supports tap.
2.  Wrap it in an `InkWell` widget to manage tap callbacks and ripple animations.

content_copy

```
// The InkWell wraps the custom flat button widget.
InkWell(
  // When the user taps the button, show a snackbar.
  onTap: () {
    ScaffoldMessenger.of(context).showSnackBar(const SnackBar(
      content: Text('Tap'),
    ));
  },
  child: const Padding(
    padding: EdgeInsets.all(12),
    child: Text('Flat Button'),
  ),
)
```
