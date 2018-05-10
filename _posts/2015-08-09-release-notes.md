---
layout: page
title: "Release Notes"
category: doc
date: 2015-05-21 23:30:46
order: 2
---

<script>
  (function (w,i,d,g,e,t,s) {w[d] = w[d]||[];t= i.createElement(g);
    t.async=1;t.src=e;s=i.getElementsByTagName(g)[0];s.parentNode.insertBefore(t, s);
  })(window, document, '_gscq','script','//widgets.getsitecontrol.com/59849/script.js');
</script>

<!-- Begin Cookie Consent plugin by Silktide - http://silktide.com/cookieconsent -->
<script type="text/javascript">
    window.cookieconsent_options = {"message":"This website uses cookies to ensure you get the best experience on our website","dismiss":"Got it!","learnMore":"More info","link":null,"theme":"dark-top"};
</script>

<script type="text/javascript" src="//s3.amazonaws.com/cc.silktide.com/cookieconsent.latest.min.js"></script>
<!-- End Cookie Consent plugin -->
<!-- 
<script type="text/javascript">
    window.doorbellOptions = {
        appKey: 'f6ciDeNxz1cbW2TSirLv5hn5btBo353HB6xTkaTvJOCDW5JlJtB1dpkaaGGg6Alb'
    };
    (function(d, t) {
        var g = d.createElement(t);g.id = 'doorbellScript';g.type = 'text/javascript';g.async = true;g.src = 'https://embed.doorbell.io/button/1824?t='+(new Date().getTime());(d.getElementsByTagName('head')[0]||d.getElementsByTagName('body')[0]).appendChild(g);
    }(document, 'script'));
</script> -->

<script>
    window['_fs_debug'] = false;
    window['_fs_host'] = 'fullstory.com';
    window['_fs_org'] = '5AXDS';
    window['_fs_namespace'] = 'FS';
    (function(m,n,e,t,l,o,g,y){
        if (e in m && m.console && m.console.log) { m.console.log('FullStory namespace conflict. Please set window["_fs_namespace"].'); return;}
        g=m[e]=function(a,b){g.q?g.q.push([a,b]):g._api(a,b);};g.q=[];
        o=n.createElement(t);o.async=1;o.src='https://'+_fs_host+'/s/fs.js';
        y=n.getElementsByTagName(t)[0];y.parentNode.insertBefore(o,y);
        g.identify=function(i,v){g(l,{uid:i});if(v)g(l,v)};g.setUserVars=function(v){g(l,v)};
        g.identifyAccount=function(i,v){o='account';v=v||{};v.acctId=i;g(o,v)};
        g.clearUserCookie=function(c,d,i){if(!c || document.cookie.match('fs_uid=[`;`]*`[`;`]*`[`;`]*`')){
        d=n.domain;while(1){n.cookie='fs_uid=;domain='+d+
        ';path=/;expires='+new Date(0).toUTCString();i=d.indexOf('.');if(i<0)break;d=d.slice(i+1)}}};
    })(window,document,window['_fs_namespace'],'script','user');
</script>


#### 2017-11-06
Version Code: <b>1001003</b> &#124; Version Short Name: <b>10.1.0-3</b>

- Enhancements and new features
	- Full compatibility with Android Oreo 8.0
	- Manually check for firmware updates
	- Custom router icons
	- Automatic speed tests and display results in either bits or bytes
	- Prevent routers from being deleted accidentally
	- Update to overall look and feel
	- Experimental Support for Tomato firmware: added more features

- Bug, reliability &amp; performance fixes
	- Fixed issue with clients list not displaying under certain circumstances
	- Router list was being reordered whenever an entry was updated
	- Battery-efficient background jobs



#### 2017-05-14
Version Code: <b>905000</b> &#124; Version Short Name: <b>9.0.5</b>

- Bug, reliability &amp; performance fixes
	- Fixed resolution of public IP addresses
	- Fixed an issue with some hosts not being displayed in the 'Clients list'
	- Fixed an issue with 'DD-WRT Beta Builds notification', sometimes not displaying
	- Addressed few memory leaks

<u>NOTE</u>: The product roadmap for this app is now public.
Visit <a href="https://ddwrt-companion.app/roadmap">https://ddwrt-companion.app/roadmap</a> to vote for the features you would like to have supported.
As always, feel free to submit feature requests at apps+ddwrt@rm3l.org



#### 2017-02-20
Version Code: <b>903000</b> &#124; Version Short Name: <b>9.0.3</b>

- Bug, reliability &amp; performance fixes
	- Fixed an issue with some hosts not being displayed in the 'Clients list'. This has been rewritten from the ground up with performance in mind
	- Fixed an issue with WAN Traffic monitoring ending at the 28th of each month
	- Fixed an issue with toggling Access Policies on some devices: you are now able to explicitly force-enable/disable policies on demand

- New features
	- Experimental Support for Tomato firmware. This is still highly experimental, and not all features are supported.
	- Update to overall app look



#### 2017-01-04
Version Code: <b>804000</b> &#124; Version Short Name: <b>8.0.4</b>

Happy New Year 2017!

- Bug, reliability &amp; performance fixes
	- Syslog tile has been rewritten from the ground up, with a focus on usability
	- Fixed few memory leaks
	- Fixed potential router connection issues

- New features
	- Notifications of new DD-WRT Build updates
	- Ability to reorder list of routers, plus Swipe-To-Remove behaviour
	- Android N compatibility: app shortcuts
	- NFC-sharing of WiFi Networks (for compatible devices)
	-  Auto-Refresh (see individual Router Settings)



#### 2016-09-21
Version Code: <b>710052</b> &#124; Version Short Name: <b>7.1.0</b>

- Bug, reliability &amp; performance fixes
	- Fixed Access Control Filter bug: filter no longer changed to 'Deny'
	- Fixed bandwidth monitoring data retrieval

- New features
	- New logo : the app has a cleaner logo
	- Security
		- This was a popular request: you are now able to PIN-protect the app. Head to the global settings to manage the PIN lock
	- 3rd party integration
		- I am working on allowing external interactions with the app. For now, this is limited to a new '<a href="https://play.google.com/store/apps/details?id=org.rm3l.ddwrt.tasker" target="_blank">DD-WRT Companion Tasker Plugin</a>' app, available for download. It allows to automate the act of launching actions against your remote routers.
		- Again, as security matters, this is entirely in your control. You can disable such feature from the global settings.
	- Redesigned the WAN bandwidths graphs, which are now easier to read and use
	- Sending feedbacks from within the app now easier, with the ability to annotate screen captures and attach logs



#### 2016-08-02
Version Code: <b>704001</b> &#124; Version Short Name: <b>7.0.4</b>

This release essentially contains bug fixes:

- Bug, reliability &amp; performance fixes
	- Fixed Java errors that sometimes happened when trying to connect to routers
	- Fixed IP geolocation feature: maps now show up correctly
	- In the "Add Router" wizard, router names are no longer validated against strict DNS patterns. The reason behind this is, even if they are not valid DNS names, they might be resolvable within a local LAN context



#### 2016-07-06
Version Code: <b>703001</b> &#124; Version Short Name: <b>7.0.3</b>

- Bug, reliability &amp; performance fixes
	- Fixed issue with clients list not displaying: MAC addresses resolution now done in the background
	- Dialogs for managing routers rewritten from the ground up: now as a step-by-step wizard
	- Charts are more readable now

- New features
	- App indexing from your Google App
	- Admin Web page now available right from the app
	- Active IP Connections redesigned, with a Stats section
	- More Material Design experience
		- New look and feel. Sending feedbacks is also now easier than ever



#### 2016-02-05
Version Code: <b>601000</b> &#124; Version Short Name: <b>6.0.1</b>

- Bug, reliability &amp; performance fixes
	- Addressed potential battery drain issues
	- Improved support of Android Marshmallow's new permissions model
	- More Material Design experience

- New features
	- Introducing Access Restrictions (Parental Control). For now, you have the ability to toggle WAN Access policies. More features will be added in upcoming versions.
	- Run Speed Tests and geolocate IPs. Measure WAN Ping (Latency) and WAN Download against servers located worldwide. You can either pick a specific server location in the settings, choose a Random one or let the app auto-select one (the one with the lowest latency). WAN Upload is to come very soon.
	- Manage local aliases, with the ability to Import and Export them. This may be of help when upgrading from the Lite to the full-featured version of the app. See the Actions Menu Item.
	- More actions: clear ARP & DNS caches, toggle HTTPd (web server)
	- Introducing Home Launcher Screen shortcuts, to get a quick access to your routers
	- OpenVPN and PPTP Clients may now be toggled in a mutually exclusive manner. For example, if you choose to disable the PPTP Client, the app will also suggest you disable the OpenVPN Client at the same time.



#### 2015-12-01
Version Code: <b>511000</b> &#124; Version Short Name: <b>5.1.1</b>

- Bug and performance fixes


#### 2015-11-27
Version Code: <b>510001</b> &#124; Version Short Name: <b>5.1.0</b>

- Bug, reliability &amp; performance fixes
	- Fixed issue with clients list not displaying on some devices
	- Made SSH connections more reliable
	- Address potential battery drain issues.
		- Among other strategies, auto-refresh is now deprecated, and you need to pull to manually refresh data whenever needed


- New features
	- Added the ability to specify custom WAN Monthly Cycle start day
	- More material design experience


#### 2015-11-05
Version Code: <b>500000</b> &#124; Version Short Name: <b>5.0.0</b>

- Bug, reliability &amp; performance fixes
	- Fixed potential "Force Close" issues when opening a given router details
	- Address potential battery drain issues
		- Global Background Service default frequency increased to 6 hours
		- Per-router "auto-refresh" default frequency increased to 1 hour
			- You now have the ability to manually refresh the router data whenever needed


- New features
	- Support for Android Marshmallow 6.0
	- More Wireless Settings
		- Ability to edit Wireless Security Settings: you can now change the passwords of your wireless networks
		- Ability to toggle wireless interfaces states: you can manually bring them up or down
	- WAN Traffic Overview Tile allows to switch between a monthly view or daily view: current day / current month
	- Ability to manually refresh router data, using a "Pull To Refresh" gesture
	- More material design experience
		- Completely redesigned the left side menu, so you can get a quick access to your routers and the menu items



#### 2015-09-18
Version Code: <b>400000</b> &#124; Version Short Name: <b>4.0.0</b>

- Bug, reliability &amp; performance fixes
	- Review &amp; clean-up app permissions
		- NOTE: Many of you have reported intrusive permissions requests from 3.3.0 version, such as Location and Identity. Those permissions were inadvertently inherited from some third-party libraries used throughout the app. As they are not relevant whatsoever for this app, they have been removed. For your information, <a href="https://help.ddwrt-companion.app/android/permissions.html">this page</a> lists the sole permissions required by the app. Thanks for your feedbacks.
	- WAN monitoring graphs now fixed
	- Fixed data retrieval issues on some devices

- New features
	- Overview tiles for having useful information at a glance:
		- A simple network topology map
		- Router Uptime
		- WAN Total traffic for the current month
	- Notifications for WAN/Public IP changes - can also show up on Android Wear
	- Details about OpenVPN Server, PPTP Client and Server, Syslog: with On/Off toggles
	- Wireless Radio On/Off toggle button
	- DHCP Release/Renew action
	- More material design experience


#### 2015-08-04
Version Code: <b>330000</b> &#124; Version Short Name: <b>3.3.0</b>

- Bug, reliability &amp; performance fixes
	- Connected Hosts Bandwidth graphs now fixed
	- Fixed data retrieval issues on some devices
	- Fixed an issue with the "Add Router" dialog stuck at the password field.

- New features
	- Local SSID lookup, with the ability to auto-detect networks. 
		- When adding/editing a router entry, you can specify a set of alternate IP/DNS to use. 
		- The app automagically makes use of the specified IP/DNS/port as soon as it detects a connection to the WiFi network specified
	- Notifications for connected clients - can also show up on wearable devices
	- More material design experience



#### 2015-06-05
Version Code: <b>320014</b> &#124; Version Short Name: <b>3.2.0</b>

- Bug, reliability &amp; performance fixes
	- Issue when installing both Lite & Premium versions
	- Wireless Ifaces &amp; Clients list sometimes not displaying
- New features
	- Dedicated Help menu item
	- Backup/Share &amp; Restore Router configuration (see Actions menu)
	- Manage WAN Monthly Traffic Monitoring
		- Switch on/off
		- Backup/Share &amp; Restore Traffic Data
			- Backup Raw file or as a CSV file
			- Share Backup files (e.g., via Gmail, Drive, ...)


#### 2015-05-02
Version Code: <b>311000</b> &#124; Version Short Name: <b>3.1.1</b>

- Bug, reliability and performance fixes
- Enhancements
	- Introducing Bulk Actions (e.g., reboot all routers listed or a given selection): accessible from the Routers list window
	- Add help link to instructions on how to setup SSH on a given DD-WRT Router
	- Backup more and more items through Android's Backup Service


#### 2015-04-27
Version Code: <b>310008</b> &#124; Version Short Name: <b>3.1.0</b>

- Bug, reliability and performance fixes
- Enhancements
	- Wake on LAN (+ Wake on LAN Daemon Settings) now available as a separate menu item/tab
	- Beautiful Home Screen Widgets: actions on Router + Wake on LAN. More to come in future releases.
	- Enhance the use of the Android's Backup Service so as to provide a restore point for the app data and settings


#### 2015-03-29
Version Code: <b>304000</b> &#124; Version Short Name: <b>3.0.4</b>

- Bug, reliability and performance fixes
	- Hotfix app crash when trying to edit or duplicate a router


#### 2015-03-29
Version Code: <b>303001</b> &#124; Version Short Name: <b>3.0.3</b>

- Bug, reliability and performance fixes
	- Fix app crashes when trying to edit or duplicate a router
	- Fix WLAN ifaces retrieval issues for Atheros chipsets
	- Fix Connected Hosts retrieval issues for some devices
- Enhancements
	- Restructure app navigation drawer menu items
	- Display detailed progress bar when retrieving connected hosts
	- Add Search views in routers and IP Connections lists
	- Leverage Android's Backup Service so as to provide a restore point for the app data and settings


#### 2015-03-23
Version Code: <b>302001</b> &#124; Version Short Name: <b>3.0.2</b>

- Regression fixes


#### 2015-03-22
Version Code: <b>300000</b> &#124; Version Short Name: <b>3.0.0</b>

- Bug, reliability and performance fixes
	- Fix WLAN Interfaces retrieval issues for Atheros chipsets
	- Fix Connected Hosts retrieval issues for some devices
- New features
	- Redesigned the navigation menu, to easily switch from one router to another
	- 'Admin>Commands' tab, to issue any commands
	- 'Toolbox' menu item: include network diagnostics utilities (ping, traceroute, nslookup, ...)
	- Active IP Connections redesign + pie chart (to see top IP destinations, and top local IP hosts)


#### 2015-03-04
Version Code: <b>211003</b> &#124; Version Short Name: <b>2.1.1</b>

- Bug fixes on some specific devices


#### 2015-03-03
Version Code: <b>210001</b> &#124; Version Short Name: <b>2.1.0</b>

- Bug, reliability and performance fixes
	- Redesigned WAN traffic charts for a better usability
	- Fix WLAN Interfaces retrieval issues for Atheros routers
	- Fix Connected Hosts retrieval issues for some devices
- New features
	- Setting to have finer control over the app network usage
	- Share WAN Traffic chart and daily breakdown
	- Added an icon for wireless clients
	- Added RSSI, Signal Strength and SNR for wireless clients
	- Ability to see Active IP Connections (overall and per-client)


#### 2015-02-09
Version Code: <b>200002</b> &#124; Version Short Name: <b>2.0.0</b>

- Bug, reliability and performance fixes
- New features
	- Material Design UI, with Dark and Light themes
	- Realtime graphs for clients bandwidth usage (resolution of at most 5 seconds)
	- Autocomplete suggestions in OpenVPN Client settings form. Suggestions are based upon what you previously entered in the form.


#### 2015-01-31
Version Code: <b>130016</b> &#124; Version Short Name: <b>1.3.0</b>

- Bug, reliability and performance fixes
	- Fix crash on LG and Nexus devices
	- WOL packets are now sent from the router, not from the smartphone/tablet
- New features
	- Per-Client Bandwidth Real-time Usage
		- Bandwidth Usage
		- Ability to filter and/or Sort
		- Ability to set a local alias for each of the Devices listed
		- Ability to manage WAN (Internet) access: you can enable or disable Internet access on a per-client basis
	- Detailed Mem and CPU Infos, by clicking on the corresponding tiles


#### 2015-01-16
Version Code: <b>121000</b> &#124; Version Short Name: <b>1.2.1</b>

- Bug, reliability and performance fixes
	- Fix crash on LG and Nexus devices


#### 2015-01-15
Version Code: <b>120004</b> &#124; Version Short Name: <b>1.2.0</b>

- Bug, reliability and performance fixes
	- Better SSH connection handling
- New features
    - Add Remote Actions: Reboot router or hard-reset router (restore factory defaults)
    - Wake on LAN (WOL) support
    - WiFi QR-Codes: you now no longer need to share your WiFi password. Just share the QR Code generated for instant connection (using a compatible scanner app)
    - OpenVPN Client settings editing: for example, you can change the target VPN server


#### 2015-01-03
Version Code: <b>110000</b> &#124; Version Short Name: <b>1.1.0</b>

- Bug, reliability and performance fixes
- New features
    - Clicking on a Wireless client Device (in 'Status > Wireless > Clients' tab) now opens up a page where we can see the device network card manufacturer (if available)
    - Add a new Dark theme, with a per-router ability to switch between Light and Dark themes
    - Add VPN logs
    - Add a new "Admin Area" menu item: NVRAM variables listing and editing
    - Add the ability to share NVRAM variables as a file


#### 2014-12-21
Version Code: <b>100015</b> &#124; Version Short Name: <b>1.0.0</b>

- Bug fixes


#### 2014-12-21
Version Code: <b>100012</b> &#124; Version Short Name: <b>1.0.0</b>

- Bug fixes


#### 2014-12-20
Version Code: <b>100010</b> &#124; Version Short Name: <b>1.0.0</b>

- Initial Release
