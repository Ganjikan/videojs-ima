<!-- GENERATED FROM SOURCE -->

# player.ima


---

## INDEX

- [METHODS](#methods)
  - [addContentAndAdsEndedListener](#addcontentandadsendedlistener-listener-)
  - [addContentEndedListener](#addcontentendedlistener-listener-)
  - [addEventListener](#addeventlistener-event-callback-)
  - [getAdsManager](#getadsmanager)
  - [initializeAdDisplayContainer](#initializeaddisplaycontainer)
  - [pauseAd](#pausead)
  - [playAdBreak](#playadbreak)
  - [requestAds](#requestads)
  - [resumeAd](#resumead)
  - [setAdBreakReadyListener](#setadbreakreadylistener-listener-)
  - [setContent](#setcontent-contentsrc-adtag-playonload-)
  - [setContentWithAdTag](#setcontentwithadtag-contentsrc-adtag-playonload-)
  - [setContentWithAdsResponse](#setcontentwithadsresponse-contentsrc-adsresponse-playonload-)
  - [setShowCountdown](#setshowcountdown-showcountdownin-)
  - [start](#start)
  - [startFromReadyCallback](#startfromreadycallback)

---

## METHODS

### addContentAndAdsEndedListener( listener )
> Adds a listener that will be called when content and all ads have
> finished playing.

##### PARAMETERS: 
* __listener__ `function` The listener to be called when content and ads complete.

_defined in_: [src/videojs.ima.js#L806](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L806)

---

### addContentEndedListener( listener )
> Adds a listener for the 'ended' event of the video player. This should be
> used instead of setting an 'ended' listener directly to ensure that the
> ima can do proper cleanup of the SDK before other event listeners
> are called.

##### PARAMETERS: 
* __listener__ `function` The listener to be called when content completes.

_defined in_: [src/videojs.ima.js#L797](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L797)

---

### addEventListener( event, callback )
> Ads an EventListener to the AdsManager. For a list of available events,
> see
> https://developers.google.com/interactive-media-ads/docs/sdks/html5/v3/apis#ima.AdEvent.Type

##### PARAMETERS: 
* __event__ `google.ima.AdEvent.Type` The AdEvent.Type for which to listen.
* __callback__ `function` The method to call when the event is fired.

_defined in_: [src/videojs.ima.js#L699](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L699)

---

### getAdsManager()
> Returns the instance of the AdsManager.

##### RETURNS: 
* `google.ima.AdsManager` The AdsManager being used by the plugin.

_defined in_: [src/videojs.ima.js#L709](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L709)

---

### initializeAdDisplayContainer()
> Initializes the AdDisplayContainer. On mobile, this must be done as a
> result of user action.

_defined in_: [src/videojs.ima.js#L135](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L135)

---

### pauseAd()
> Pauses the ad.

_defined in_: [src/videojs.ima.js#L821](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L821)

---

### playAdBreak()
> Called by publishers in manual ad break playback mode to start an ad
> break.

_defined in_: [src/videojs.ima.js#L306](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L306)

---

### requestAds()
> Creates the AdsRequest and request ads through the AdsLoader.

_defined in_: [src/videojs.ima.js#L143](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L143)

---

### resumeAd()
> Resumes the ad.

_defined in_: [src/videojs.ima.js#L832](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L832)

---

### setAdBreakReadyListener( listener )
> Sets the listener to be called to trigger manual ad break playback.

##### PARAMETERS: 
* __listener__ `function` The listener to be called to trigger manual ad break playback.

_defined in_: [src/videojs.ima.js#L814](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L814)

---

### setContent( contentSrc, adTag, playOnLoad )
> DEPRECATED: Use setContentWithAdTag.
> Sets the content of the video player. You should use this method instead
> of setting the content src directly to ensure the proper ad tag is
> requested when the video content is loaded.

##### PARAMETERS: 
* __contentSrc__ `?string` The URI for the content to be played. Leave
* __adTag__ `?string` The ad tag to be requested when the content loads.
* __playOnLoad__ `?boolean` True to play the content once it has loaded,

_defined in_: [src/videojs.ima.js#L725](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L725)

---

### setContentWithAdTag( contentSrc, adTag, playOnLoad )
> Sets the content of the video player. You should use this method instead
> of setting the content src directly to ensure the proper ad tag is
> requested when the video content is loaded.

##### PARAMETERS: 
* __contentSrc__ `?string` The URI for the content to be played. Leave
* __adTag__ `?string` The ad tag to be requested when the content loads.
* __playOnLoad__ `?boolean` True to play the content once it has loaded,

_defined in_: [src/videojs.ima.js#L743](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L743)

---

### setContentWithAdsResponse( contentSrc, adsResponse, playOnLoad )
> Sets the content of the video player. You should use this method instead
> of setting the content src directly to ensure the proper ads response is
> used when the video content is loaded.

##### PARAMETERS: 
* __contentSrc__ `?string` The URI for the content to be played. Leave
* __adsResponse__ `?string` The ads response to be requested when the
* __playOnLoad__ `?boolean` True to play the content once it has loaded,

_defined in_: [src/videojs.ima.js#L760](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L760)

---

### setShowCountdown( showCountdownIn )
> Changes the flag to show or hide the ad countdown timer.

##### PARAMETERS: 
* __showCountdownIn__ `boolean` Show or hide the countdown timer.

_defined in_: [src/videojs.ima.js#L907](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L907)

---

### start()
> DEPRECATED: Use startFromReadyCallback
> Start ad playback, or content video playback in the absence of a
> pre-roll.

_defined in_: [src/videojs.ima.js#L233](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L233)

---

### startFromReadyCallback()
> Start ad playback, or content video playback in the absence of a
> pre-roll. **NOTE**: This method only needs to be called if you provide
> your own readyCallback as the second parameter to player.ima(). If you
> only provide options and do not provide your own readyCallback,
> **DO NOT** call this method. If you do provide your own readyCallback,
> you should call this method in the last line of that callback. For more
> info, see this method's usage in our advanced and playlist examples.

_defined in_: [src/videojs.ima.js#L248](https://github.com/googleads/videojs-ima/blob/mastersrc/videojs.ima.js#L248)

---

