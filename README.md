  
# Packaging an app, starting from this example

- Copy this app before working on it, using the ['Use this template'](https://github.com/YunoHost/example_ynh/generate) button on the Github repo.
- Edit the `manifest.json` with app specific info.
- Edit the `install`, `upgrade`, `remove`, `backup`, and `restore` scripts, and any relevant conf files in `conf/`.
  - Using the [script helpers documentation.](https://yunohost.org/packaging_apps_helpers)
- Add a `LICENSE` file for the package.
- Edit `doc/DISCLAIMER*.md`
- The `README.md` files are to be automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator


---

<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Nonbiri for YunoHost

[![Integration level](https://dash.yunohost.org/integration/example.svg)](https://dash.yunohost.org/appci/app/example) ![](https://ci-apps.yunohost.org/ci/badges/example.status.svg)  ![](https://ci-apps.yunohost.org/ci/badges/example.maintain.svg)
[![Install example with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=example)

*[readme](./README_fr.md)*

> *This package allows you to install example quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

![Nonbiri](https://raw.githubusercontent.com/rs1703/nonbiri/gh-pages/1.png)

_The UI is inspired by [Tachiyomi](https://github.com/tachiyomiorg/tachiyomi) (Please use that if you want to read manga on mobile devices)._

# Nonbiri

Nonbiri is a self-hosted back-end and front-end for MangaDex. Just something I made for myself because MangaDex's new UI is bloated piece of hot garbage. The back-end itself is lightweight because of Go's garbage collector (< 100MB).

![Memory usage](https://raw.githubusercontent.com/rs1703/nonbiri/gh-pages/2.png)

## Features

- Online/offline read and browse MangaDex
- History tracker and scheduled updates
- Chapters and covers are automatically downloaded/cached forever
- Real-time synchronization between tabs/browsers and computers
- Long strip, right-to-left and left-to-right reading modes
- Customizable keyboard shortcuts for navigating between pages and chapters

Library and history are stored locally, Nonbiri will not push follows and reading history to MangaDex for obvious reasons.


## License

**Nonbiri** is licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

## Disclaimer

The developer of this application does not have any affiliation with the content providers available.

**Shipped version:** 1.0~ynh1

**Demo:** https://demo.example.com


## Screenshots


   ![](./doc/screenshots/example.jpg)




## Disclaimers / important information

* Any known limitations, constrains or stuff not working, such as (but not limited to):
    * requiring a full dedicated domain ?
    * architectures not supported ?
    * not-working single-sign on or LDAP integration ?
    * the app requires an important amount of RAM / disk / .. to install or to work properly
    * etc...

* Other infos that people should be aware of, such as:
    * any specific step to perform after installing (such as manually finishing the install, specific admin credentials, ...)
    * how to configure / administrate the application if it ain't obvious
    * upgrade process / specificities / things to be aware of ?
    * security considerations ?



## Documentation and resources

* Official app website: https://example.com
* Official user documentation: https://yunohost.org/apps
* Official admin documentation: https://yunohost.org/packaging_apps
* Upstream app code repository:  https://some.forge.com/example/example
* YunoHost documentation for this app: https://yunohost.org/app_example
* Report a bug: https://github.com/YunoHost-Apps/example_ynh/issues

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/example_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/example_ynh/tree/testing --debug
or
sudo yunohost app upgrade example -u https://github.com/YunoHost-Apps/example_ynh/tree/testing --debug
```

**More info regarding app packaging:** https://yunohost.org/packaging_apps