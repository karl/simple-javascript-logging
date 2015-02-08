# Simple JavaScript Logging

A simple javascript logging framework.

Javascript Logging provides an unobtrusive way of debugging your javascript. A small expandable div positioned in the top left corner of your page displays the logs. Any errors logged using logError(e) automatically expand the log, providing instant feedback when something goes wrong. Logging can be turned off for production systems without having to remove all the logging code.

## Screenshot

TODO: Add screenshot

## Download

The [Simple JavaScript logging framework is available on GitHub](https://github.com/karl/simple-javascript-logging).

## Usage

In Your HTML

<script language="JavaScript" type="text/javascript" src="js/logging.js"></script>

In Your Javascript

try {
  // ...
  log('value of foo: ' + foo);
  //...
  } catch(e) {
    logError(e);
  }

  Options

  // The log will no longer be created or displayed
  loggingDisplay = false;

  // The log will start expanded
  loggingStartExpanded = true;

  // The location where javascript logging was unzipped to
  // so that the CSS + additional javascript can be loaded
  LOGGING_BASE = '/javascript-logging/';
