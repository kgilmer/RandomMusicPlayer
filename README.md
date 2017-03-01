# RandomMusicPlayer

This repo is an adaptation of https://github.com/android/platform_development/tree/master/samples/RandomMusicPlayer.  It's being used here to experiment with Android audio APIs.

## Branches

### `original`
The original source code from the repo above.  This branch does not compile, there is no build file.  It's mainly here for reference and being able to easily diff.

### `original_runtime_perms`
The original source code with minor updates including a gradle build file, moving of source files into the gradle scheme, and API updates necessary to compile and run on modern Android.

### `exoplayer`
The true purpose of this repo is to evaluate the API complexity of Google's ExoPlayer.  The MediaPlayer code was removed and substituted with ExoPlayer.

## Status
`original_runtime_perms` and `exoplayer` build and run.  There are probably some things I've missed, but generally they work as expected.

## How to build

Change to `original_runtime_perms` or `exoplayer` and build as you would any other gradle-based Android project.

## Original README

A simple music player that illustrates how to make a multimedia application
that manages media playback from a service. It allows the user to play music
available on the device or specify a URL from which the media should be
streamed.  It also illustrates how to use the notification system to indicate
an ongoing task and how to deal with audio focus changes.</p>

### Update
This sample also illustrates how to use the
<code><a href="../../../reference/android/media/RemoteControlClient.html">RemoteControlClient</a></code>
class added in API level 14 to integrate with music playback remote controls
such as those found on the lockscreen.
