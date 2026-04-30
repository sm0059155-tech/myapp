
# Layam Offline iOS App Blueprint

## Overview

The goal is to create a simple, offline-capable iOS application that displays the content of the existing `layam.html` file. This will be achieved by embedding a webview within a Flutter application.

## Core Implementation

- **Framework**: Flutter
- **Webview Plugin**: `flutter_inappwebview` will be used for its robust feature set and support for loading local files.
- **Asset Management**: The `layam.html` file and its associated resources will be bundled as application assets.

## Implemented Features

- **Webview Integration**: The main screen of the application will consist of a full-screen webview.
- **Offline Content**: The webview will load `layam.html` directly from the app's bundled assets, allowing it to function without an internet connection.
- **JavaScript and Media**: The webview will be configured to allow JavaScript execution and inline media playback, which are necessary for the audio features in `layam.html`.

## Plan for Current Request

1.  **Add Dependencies**: Add the `flutter_inappwebview` package to `pubspec.yaml`.
2.  **Organize Assets**:
    *   Copy the `layam.html` file to the `assets/` directory.
    *   Update the `pubspec.yaml` file to ensure `assets/layam.html` is included in the application bundle.
3.  **Develop Webview UI**:
    *   Replace the contents of `lib/main.dart`.
    *   The new code will initialize the app and create a screen containing an `InAppWebView` widget.
    *   The webview will be configured to load `assets/layam.html`.
4.  **Finalization**: Provide a summary of the changes and instructions on how to run the new application.
