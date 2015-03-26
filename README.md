# adblock-meets-privoxy-miniweb

Easiest setup for replacing AdBlock which is a memory hog with MUCH lighter setup based on privoxy. Keep your memory consumption at bay.


This setup guide is intended for MS Windows 7 and above.

Lazy guide (see full guide below for building your own filter list, etc.)
1. Install [Privoxy](http://www.privoxy.org/)
2. Install lighttpd or apache or [nginx](http://nginx.org/en/docs/windows.html)
3. Update web server config: https://projects.zubr.me/wiki/adblock2privoxy
4. Update privoxy settings
````
actionsfile ab2p.system.action
actionsfile ab2p.action
filterfile ab2p.system.filter
filterfile ab2p.filter
````
5. Grab prebuilt Adblock filters list [Privoxy dir](https://dl.dropboxusercontent.com/u/19020828/privoxy_conf.7z), [Web server filters](https://dl.dropboxusercontent.com/u/19020828/privoxy_css.7z)
6. Add filter update script to your Task Scheduler or Startup folder so it runs from time to time.

Full guide:
1. Install [Privoxy](http://www.privoxy.org/)
2. Install lighttpd or apache or [nginx](http://nginx.org/en/docs/windows.html)
3. Update web server config
4. Update privoxy settings:
5. Create a set of your own blocking [filters](http://easylist.adblockplus.org/)
6. Run adblock2privoxy every once in a while
