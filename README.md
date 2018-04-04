# Electron offscreen webview crash demo

This is a demo for a [bug in Electron](https://github.com/electron/electron/issues/12528),
where an offscreen webview will crash electron (At least on windows).

# Important notes

* Because the issue only applies to webviews, I am using a webview that loads
google's homepage and focuses the text box. If google moves the text box, then
this will no longer work right.

* When you run the app, there is no output, because it's an offscreen window.
That is an important part of this bug. If the window is not rendered offscreen,
everything works properly.

* I will update this repo to include extra information as I uncover it.
