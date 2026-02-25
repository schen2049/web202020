# Requirements

## Summary

A user must be able to configure a timer to trigger a notification every X seconds.
After X seconds, user receives a notification to rest their eyes.
The rest time lasts Y seconds.  After Y seconds, the cycle repeats.

## Compatibility

This app must work in Chrome and Firefox on Windows, Linux and MacOS.

## User Configuration

User must be able to configure the following
* "Time between alerts" - By default, this will be 20 minutes.  The value should be a positive integer and user must have a dropdown to select seconds, minutes or hours.
* "Rest time" - By default, this will be 20 seconds.  The value should be a positive integer and user must have a dropdown to select seconds or minnutes.

This configuration must be saved somewhere so that the user has the same settings when they reload the page.

## Display

The primary display of the app must be a large, centered timer in the format "mm:ss".  This is a countdown that cycles between the configured "Time between alerts" and "Rest time".

Above the timer must show small text that says "Ready", "Work", "Rest" or "Paused"

Buttons for user actions must be shown below the timer.

## Notification

When "Work" timer hits 0
* a notification should be shown through the browser
* a sound should play
* if the user is on a different tab than this app, the user should be brought back to this tab

## User Actions

User has 3 buttons they can click
* Start - The app starts in "Ready" state.  When Start is clicked, the timer starts running.  
* Paused - This button stops the currently active timer
* Reset - This button resets the timer to the Ready state with the given user configuration