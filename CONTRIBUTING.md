# Contributing to stacked

First of all, thank you for considering contributing to stacked.
This is an open souce project and shall be driven by the community.

This document describes how contributions may be done and what is required
to develop on stacked.

TODO -> describe workflow and stuff

## **Running using flutter devices**

Use the command:

```
flutter test integration_test/app_test.dart
```

If multiple devices was found, select the device you want to run the tests on.

## **Running using chrome driver**

Ensure you have the [chrome driver](https://chromedriver.chromium.org/downloads) installed.

Start the chrome driver:

```
chromedriver --port=4444
```

In a separate terminal, run the tests:

```
flutter drive --driver=test_driver/integration_test.dart --target=integration_test/app_test.dart -d web-server
```