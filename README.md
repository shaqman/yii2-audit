# Yii2 Audit

[![Join Chat](https://img.shields.io/badge/gitter-join%20chat-blue.svg?style=flat-square)](https://gitter.im/bedezign/yii2-audit?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Latest Version](https://img.shields.io/github/tag/bedezign/yii2-audit.svg?style=flat-square&label=release)](https://github.com/bedezign/yii2-audit/tags)
[![Software License](https://img.shields.io/badge/license-BSD-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/bedezign/yii2-audit/master.svg?style=flat-square)](https://travis-ci.org/bedezign/yii2-audit)
[![Coverage Status](https://img.shields.io/scrutinizer/coverage/g/bedezign/yii2-audit.svg?style=flat-square)](https://scrutinizer-ci.com/g/bedezign/yii2-audit/code-structure)
[![Quality Score](https://img.shields.io/scrutinizer/g/bedezign/yii2-audit.svg?style=flat-square)](https://scrutinizer-ci.com/g/bedezign/yii2-audit)
[![Total Downloads](https://img.shields.io/packagist/dt/bedezign/yii2-audit.svg?style=flat-square)](https://packagist.org/packages/bedezign/yii2-audit)
[![Yii2 Framework](https://img.shields.io/badge/powered_by-Yii2_Framework-green.svg?style=flat-square)](http://www.yiiframework.com/)

Yii2 Audit is a module that records and displays web/cli requests, database changes, php/js errors and associated data.

## Features

* Installs as a simple module so it can be added without any hassle.

* Tracks all incoming web and console request data:
  * The users IP Address and User ID.
  * URL Information including the route/params, referrer and where they were redirected to.
  * PHP SuperGlobals `$_GET`, `$_POST`, `$_SERVER`, `$_FILES` and `$_COOKIES`.
  * Headers from the Request and Response.
  * Memory Usage and Request Duration.
  * SQL Queries and Profile information.
  * Yii Logs

* You can either track specific actions and nothing else or exclude specific routes from logging (wildcard supported).

* Track database changes by implementing the `AuditTrailBehavior`.

* Automatically log JavaScript errors. Errors and warning are logged automatically (if you activate the functionality), but the javascript component also provides methods to manually add logging entries.

* Record all PHP exceptions and errors in the background.  Once logged you can configure a cron task to email the errors to a developer so issues can be fixed before they are even reported by a user.

* Track extra data using a simple method call, or by creating a new Panel.

* View your data. The module contains a nice viewer that is automatically made available when you add it to your configuration. It has configurable permissions to limit access to this functionality, both by roles or by user-id.

## Documentation

For installation, configuration and usage instructions please refer to the [Documentation](docs/).

For changes since the last version see the [Changelog](CHANGELOG.md).

## Screenshots

![Index example](docs/screenshots/audit-index.png?raw=true)
![View example](docs/screenshots/audit-view.png?raw=true)
![Diff example](docs/screenshots/audit-diff.png?raw=true)

## Credits

Thanks to [everyone who has contributed](CREDITS.md)
