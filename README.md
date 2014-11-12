Welcome to the release repository of Unity Ads SDK. To get started, make sure you have an account
registered with Applifier. If you don't have one, you can create an account at https://my.applifier.com/

For integration and generic documentation, go to https://github.com/Applifier/unity-ads/wiki

For source code access or code review, check https://github.com/Applifier/unity-ads

Unity Ads SDK is licensed under the Apache License, Version 2.0 (http://www.apache.org/licenses/LICENSE-2.0.html)

In any issues, please file in issue against https://github.com/Applifier/unity-ads/issues repository,
or log a ticket with us by emailing support@applifier.zendesk.com

Unity Ads SDK Release Notes
===========================

v1.3.10 November 12th, 2014
---------------------------

*Android*

- Allow caching videos over cellular networks

v1.3.9 October 30th, 2014
-------------------------

*Android*

- Restored runtime configuration of debug logging
- Minor fixes

*iOS*

- Minor fixes

v1.3.8 September 10th, 2014
---------------------------

*Android*

- If game sets a zone that does not exist, then treat the zone as disabled instead of falling back to default zone
- Minor bug fixes

*iOS*

- If game sets a zone that does not exist, then treat the zone as disabled instead of falling back to default zone
- Minor bug fixes

*Unity*

- Remove deprecated Unity plugin. Please use Unity Ads package from Unity Asset Store instead.

v1.3.7 August 27th, 2014
------------------------

*Android*

- Fix handling of backgrounding during video play for launch mode singleTask applications, like Unity

v1.3.6 August 19th, 2014
------------------------

*Android*

- Fix timer crashes

v1.3.5 August 12th, 2014
------------------------

*Android*

- Fix null reward item key in video completed callbacks

v1.3.4 August 12th, 2014
------------------------

*Unity*

- Fixes for Unity plugin

*Android*

- Fixes for several crashes and null pointers
- Fix issues when destroyed activity gets recreated
- Don't allow ads if there is no network connectivity

v1.3.3 July 29th, 2014
---------------------

*Android*

- Fix incorrect initialization logic to a more robust version

*iOS*

- Fail gracefully on invalid server configuration in an edge case

v1.3.2 July 21st, 2014
---------------------

*Android*

- Move to using Android advertising identifier as a primary tracking identifier 

v1.3.1 July 3rd, 2014
---------------------

*iOS*

- Fixes for ApplifierImpact compability layer
- Minor fixes

*Android*

- Fixes and improvements for Android activity handling
- Minor fixes

v1.3.0 June 11th, 2014
----------------------

Applifier Impact/Everyplay GameAds are now being fully transformed into Unity Ads SDK!
Yes, this time SDK API internals and documentation will be around for long term usage.

Migration notes: https://github.com/Applifier/unity-ads/wiki/Transition-from-Applifier-Impact-and-Everyplay-GameAds

*iOS*

- Compability layer with old ApplifierImpact interface
- Several minor bug fixes

*Android*

- Always send Google Play advertising ID (mandatory from 1st August 2014)
- Compability layer with old ApplifierImpact interface
- SDK is now available as Android library project
- Refactored SDK to use safer singleton pattern
- Several minor bug fixes

*Unity*

- Many improvements to Unity plugin integration
- Improved Android integration support
- Added a legacy cleanup script against older Applifier Impact or Everyplay GameAds plugin releases, see migration notes
- Separate game IDs for Android and iOS
- Fix for delays after closing video ad

v1.2.5 May 19th, 2014
---------------------

*Android*

- Fix video caching issue

v1.2.4 May 13th, 2014
---------------------

*Android*

- Fix issues with Unity plugin Android manifest

v1.2.3 May 8th, 2014
--------------------

*Android*

- Fix a rare race condition in video caching code

v1.2.2 May 6th, 2014
--------------------

*iOS*

- Fix release build to universal binary
- Fix unneccessary asserts on invalid campaign data while using the debug build

*Android*

- Fix multiple initializations in certain cases

v1.2.1 May 2nd, 2014
--------------------

*Android*

- Fix crash when buffering over very slow connections
- Fix crash when closing end screen on certain zone configurations

v1.2.0 April 30th, 2014
-----------------------

*iOS & Android*

- Improved caching of videos
- Various fixes on both platforms

v1.1.0 February 20th, 2014
--------------------------

*iOS & Android*

- Support for multiple ad-placements with different settings for ads (aka. zones)  API
- various minor fixes on both platforms

*Android*

- Support for Android Advertising ID, requires Google Play Services libraries
- Better adplan performance on Android (New ads checked more frequently)

*iOS*

- device model detection improvements on iOS

v1.0.10 September 25th, 2013
----------------------------

*iOS:*

- Support for iOS 7

v1.0.9 July 19th, 2013
----------------------

*All platforms:*

- Added a boolean for the video completion delegate for telling whether the video was skipped or not.

*iOS:*

- Removed MAC Address and ODIN1 from iOS7 and added plain text Advertising Identifier (IDFA) sending.
- Enabled skipping stalled video.
- Fixed a bug which caused the video end event not being sent always although the user reached the end.

v1.0.8 July 5th, 2013
---------------------

*All platforms:*

- Improved video playback error handling

*iOS:*

- Moved network reachability test to background
- Removed duplicate logging events

*Unity:*

- Fixed a build error on Android
- Fixed Unity wrapper calling outdated canShow instead of canShowAds

v1.0.7 June 18th, 2013
----------------------

*All platforms:*

- Fixed reward item showing up in the offer screen. Previously it always showed the default item set on the server side. Now the item selection works on the client side, too.

v1.0.6 May 31st, 2013
---------------------

*All platforms:*

- Fixed mute button functionality when developer settable video muting was on.

v1.0.5 May 23rd, 2013
---------------------

*iOS:*

- Fixed a bug that crashed Unity Ads when user attempted to close the Unity Ads window immediately after starting video playback (Thank you First Touch Games for reporting this issue!).

*Android:*

- Fixed a bug in instrumentation where WebApp would get erroneous data from native side and log javascript errors.

v1.0.4 May 22nd, 2013
---------------------

*All platforms:*

- Support for muting video sounds & controlling the default setting from code
- Support setting Unity Ads orientation to locked or unlocked to device orientation
- Ability to skip videos after n seconds as a server side configuration
- Better handling of opening iTunes / Google Play
- Improved instrumentation of network status
- Preview capability for loading campaigns of specific advertiser for previewing campaigns on the device

*iOS:*

- Option to use a Native iOS UI instead of UIWebView in order to save memory

*Android:*

- Unity Ads no longer requires CHANGE_WIFI_STATE permission
- android:configChanges="keyboardHidden|orientation" require new possible options depending on the developers targetSdk etc. All possible options Unity Ads needs are: "keyboardHidden|orientation|screenLayout|screenSize|smallestScreenSize"

v1.0.3.2 March 13, 2013
-----------------------

*Android:*

- Support for Unity3D
- Minor edge-case bugfixes

*iOS:*

- Support for Unity3D

v1.0.3.1 February 27, 2013
--------------------------

*Android:*

- Android support is now officially released, get it while it's hot!

*iOS:*

- Bugfixes

v1.0.3 January 23, 2013
-----------------------

*iOS:*

- Support for multiple reward items


v1.0.2 December 11, 2012
------------------------

*Adobe AIR:*

- Support for Adobe AIR when running on iOS platforms

*iOS:*

- Better fallbacks in some cases if data is not received correctly

v1.0.1 November 28, 2012
------------------------

*iOS:*

- Refactored view logic for easier integration
- Bug fixes, improved cache policies for video ad caching

*Android:*

- Android version still in development, should not be used in production apps
