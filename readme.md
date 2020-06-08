# @titanium/webdialog

[![@titanium/webdialog](https://img.shields.io/npm/v/@titanium/webdialog.png)](https://www.npmjs.com/package/@titanium/webdialog)


> Native modules that allows you to use native SFSafariViewController (iOS) and Chrome Pages (Android) with Axway Titanium native mobile apps..

* [📝 Description](#-description)
* [🚀 Getting Started](#-getting-started)
  * [Install `@titanium/webdialog` in root of project](#install-titaniumwebdialog-in-root-of-project)
* [✨Features](#features)
* [API's](#apis)
  * [Top-Level](#top-level)
    * [Methods](#methods)
    * [Properties](#properties)
    * [Events](#events)
  * [`AuthenticationSession` (iOS only)](#authenticationsession-ios-only)
    * [Methods](#methods-1)
    * [Events](#events-1)
* [📚Learn More](#learn-more)
* [📣 Feedback](#-feedback)
* [©️ Legal](#️-legal)


## 📝 Description

This is a repackaging of the compiled iOS and Android modules for [ti.webdialog](https://github.com/appcelerator-modules/titanium-web-dialog) to allow for installation via npm.

## 🚀 Getting Started

### Install `@titanium/webdialog` in root of project

```
npm install @titanium/webdialog
```

## ✨Features

* [x] Includes Titanium native iOS module: `ti.webdialog 1.2.0`
* [x] Includes Titanium native Android module: `ti.webdialog 2.0.0`


## API's

### Top-Level

```javascript
const webdialog = require('@titanium/webdialog');
```

#### Methods

* `open(arguments)`
    * `url` (String)
    * `barColor` (String)
    * `animated` (Boolean, iOS only)
    * `entersReaderIfAvailable` (Boolean, iOS only)
    * `barCollapsingEnabled` (Boolean)
    * `title` (String, iOS only)
    * `tintColor` (String, iOS only)
    * `dismissButtonStyle` (`DISMISS_BUTTON_STYLE_*`, iOS only)
    * `showTitle` (Boolean, Android only)
    * `fadeTransition` (Boolean, Android only)
    * `enableSharing` (Boolean, Android only) - Enable Share... menu item to share link
    * `closeIcon` (String, Android only) - image path to show as close-button icon
  
* `isSupported()` -> Boolean
* `isOpen()` (iOS only) -> Boolean
* `close()` (iOS only)

#### Properties

* `DISMISS_BUTTON_STYLE_DONE` (iOS only)
* `DISMISS_BUTTON_STYLE_CLOSE` (iOS only)
* `DISMISS_BUTTON_STYLE_CANCEL` (iOS only)

#### Events

* `open` -> `success` (Boolean), `url` (String)
* `close` -> `success` (Boolean), `url` (String) - iOS only
* `load` -> `success` (Boolean), `url` (String) - iOS only
* `redirect` -> `url` (String) - iOS only

### `AuthenticationSession` (iOS only)

#### Methods

* `createAuthenticationSession(arguments)`
    * `url` (String)
    * `scheme` (String) 

#### Events

* `callback` -> `success` (Boolean), `callbackURL` (String)



## 📚Learn More

- [ti.webdialog GitHub Repo](https://github.com/appcelerator-modules/titanium-web-dialog) - Repo for ti.webdialog modules


## 📣 Feedback

Have an idea or a comment?  [Join in the conversation here](https://github.com/brentonhouse/titanium-webdialog/issues)! 

## ©️ Legal

Modules are licensed under Apache 2.0 from https://github.com/appcelerator-modules/titanium-web-dialog

Alloy is developed by Appcelerator and the community and is Copyright © 2012-Present by Appcelerator, Inc. All Rights Reserved.

Alloy is made available under the Apache Public License, version 2. See their license file for more information.

Appcelerator is a registered trademark of Appcelerator, Inc. Titanium is a registered trademark of Appcelerator, Inc. Please see the LEGAL information about using trademarks, privacy policy, terms of usage and other legal information at http://www.appcelerator.com/legal.