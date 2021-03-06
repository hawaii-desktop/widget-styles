Widget Styles
=============

[![IRC Network](https://img.shields.io/badge/irc-freenode-blue.svg "IRC Freenode")](https://webchat.freenode.net/?channels=hawaii-desktop)
[![GitHub release](https://img.shields.io/github/release/hawaii-desktop/hawaii-widget-styles.svg)](https://github.com/hawaii-desktop/hawaii-widget-styles)
[![GitHub issues](https://img.shields.io/github/issues/hawaii-desktop/hawaii-widget-styles.svg)](https://github.com/hawaii-desktop/hawaii-widget-styles/issues)

Styles for applications using QtQuick Controls.

## Dependencies

In order to build and install Widget Styles you need Qt 5.2 or better with
at least the following modules:

* qtbase
* qtdeclarative
* qtquickcontrols

You can either build Qt from git yourself or download binaries.

More information about building Qt 5 from can be found here:

  http://qt-project.org/wiki/Building-Qt-5-from-Git

Qt 5 binaries can be downloaded from http://qt-project.org/downloads

## Build

Building Widget Styles is a piece of cake.

Assuming you are in the source directory, just create a build directory
and run cmake:

```sh
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=/opt/hawaii ..
```

To do a debug build the last command can be:

```sh
cmake -DCMAKE_INSTALL_PREFIX=/opt/hawaii -DCMAKE_BUILD_TYPE=Debug ..
```

To do a release build instead it can be:

```sh
cmake -DCMAKE_INSTALL_PREFIX=/opt/hawaii -DCMAKE_BUILD_TYPE=Release ..
```

If not passed, the `CMAKE_INSTALL_PREFIX` parameter defaults to /usr/local.
You have to specify a path that fits your needs, /opt/hawaii is just an example.

Package maintainers would pass `-DCMAKE_INSTALL_PREFIX=/usr`.

The `CMAKE_BUILD_TYPE` parameter allows the following values:

* **Debug:** debug build
* **Release:** release build
* **RelWithDebInfo:** release build with debugging information

## Installation

It's really easy, it's just a matter of typing:

```sh
make install
```

from the build directory.
