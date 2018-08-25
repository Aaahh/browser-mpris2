# browser-mpris2
Implements the MPRIS2 interface for Firefox.

Currently, the following sites are supported with almost all of the capabilities MPRIS2 allows:
* [YouTube](https://youtube.com)
* [HookTube](https://hooktube.com)

Pull requests are welcome.

## Installation (for Firefox)
1. First, go to `about:debugging`, enable `Enable add-on debugging`, click `Load Temporary Add-on` and select manifest.json from this repo.  Notice, the extension ID.
2. Next run browser-mpris2/native/install-firefox.py
3. ???
4. Profit
5. Repeat Step 1 everytime you open firefox until this is published to the firefox addon store.

If on GNOME or similar you should be able to take advantage of your new powers immediately.  Otherwise, you can use something like [playerctl](https://github.com/acrisci/playerctl), perhaps bind it to a key or `XF86AudioPlay` and the like if your keyboard has them.
## Similar Projects
* [plasma-browser-integration](https://github.com/KDE/plasma-browser-integration)
  It's more general as it works on `<audio>` and `<video>` elements, though it misses out on some of the more "advanced" capabilities, such as cover art support.
* [shwsh/web-mpris2](https://github.com/shwsh/web-mpris2)
  A port of this extension to Tampermonkey/Greasemonkey (and WebSockets).

## TODO
* Support the (supposedly experimental) [Media Session API](https://developer.mozilla.org/en-US/docs/Web/API/Media_Session_API) that sites can use to set metadata.  plasma-browser-integration uses where available.
