# progress_dialog

A light weight package to show progress dialog

[Get the library](https://pub.dartlang.org/packages/progress_dialog) | [Example](https://pub.dartlang.org/packages/progress_dialog#-example-tab-)

## How to use

Import the package

```
import 'package:progress_dialog/progress_dialog.dart';
```
Create an instance of ProgressDialog
```
ProgressDialog pr;
```

Initialise the pr object inside the **build()** method passing context to it

```
pr = new ProgressDialog(context);
```

If need you can change the default message of progress dialog
```
pr.setMessage('Please wait...');
```
Showing the progress dialog
```
pr.show();
```

Dismissing the progress dialog
```
pr.hide();
```

Check if progress dialog is showing
```
bool isProgressDialogShowing = pr.isShowing();
```

To use a different loading widget like one from [here](https://pub.dartlang.org/packages/flutter_spinkit), use the optional parameter `loadingIndicator`, otherwise it will use the default `CircularProgessIndicator()`.
You may need to modify the default width allotted to the indicator using the optional parameter `loadingIndicatorWidth`. To change the style from Cupertino to Material,
use the optional parameter `progressDialogType` which takes an enumeration of `ProgressDialogType.Material` or `ProgressDialogType.CupertinoStyle`
```
ProgressDialog(context, loadingIndicator: Widget, loadingIndicatorWidth: double, progressDialogType: ProgressDialogType)
```

## Demo
<img src="https://raw.githubusercontent.com/fayaz07/progress_dialog/master/progress.gif" width="350" height="620" alt="ProgressDialog Demo" />



