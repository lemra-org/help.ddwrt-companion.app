---
layout: page
title: "Permissions"
category: android
date: 2015-08-08 22:29:14
order: 1
disqus: 1
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

When you install any software on an Android device, Android will declare all the functions that the software is capable of, such as accessing your camera, contacts or location. Each permission is accompanied with a brief description to offer an understanding for what it may be used for. In order to install the software, you must acknowledge that you are aware of what the software is capable of by giving Android your permission.

In other words, if you install the DD-WRT Companion app, you should be presented a screen letting you know that the app is asking for your permission to access information or use features from your Android phone or tablet. 

Keep in mind that Android controls the way the permissions are named, and the way they are named does not necessarily reflect how the app and other apps use them.

Below you will find an exhaustive list of the permissions we currently request for the DD-WRT Companion app on Android, as well as an example of how we use each one. This list is meant to give you a better understanding of how the app uses these permissions. 
If you've already installed the app, you can find a list of the permissions the app uses in your phone or tablet's Applications Manager, or by visiting the <a href="https://play.google.com/store/apps/details?id=org.rm3l.ddwrt">Play Store</a> and clicking <b>View Details</b> under <b>Permissions</b>.

Note that the names of these permissions and how they are displayed on your device may differ depending upon the version of Android you are using.

We may update this list as we keep enriching the app with additional capabilities that may require new permissions. So please check back here to learn more about which permissions we request and how we use them. 
<br/><br/>

#### Internet - Full network access
We use network access to:
<ul>
<li>establish remote SSH connections to your routers, obviously</li>
<li>gather and privately upload your valuable feedback to dedicated backends hosted on https://doorbell.io and https://aws.amazon.com/s3/</li>
<li>retrieve your router public IP address on the Internet, using http://icanhazip.com , if allowed in the router settings </li>
<li>resolve MAC addresses, via a dedicated backend on http://tools.rm3l.org</li>
<li>lookup and geolocate IP Addresses via https://dazzlepod.com</li>
<li>fetch your router avatars on http://cloudinary.com</li>
<li>leverage the Android's Backup Service so as to provide a restore point for the app data and settings</li>
<li>report crash errors to dedicated backends hosted on http://www.tracepot.com and https://fabric.io, provided you allowed it in the app preferences</li>
<li>fetch ads, in the Lite version of the app</li>
<li>provide the "Help" menu, which currently displays this website (http://help.ddwrt-companion.rm3l.org)</li>
</ul>



#### View Network connections
We use this permission in conjunction with the "Full network access" permission, as it allows the app to detect whether an active network connection is available when trying to retrieve/push data from/to the router.



#### View Wi-Fi connections
This is essentially useful for the "Local SSID Lookup" feature. It allows the app to view whether a Wi-Fi is enabled and use any user-defined alternate IP/DNS/port to connect to the router.



#### Run at startup
We run at startup if you choose to enable the Background Service in the app preferences. 
This way, the app can perform the following actions in background (i.e., even if you never open the app per se):
<ul>
<li>display notifications about devices connected to your router(s)</li>
<li>display notifications about public and WAN IP addresses changes</li>
</ul>
The frequency at which this background service synchronizes with the router is controlled by you in the preferences.


#### Prevent phone from sleeping
This is used by the Background Service, if enabled in the app preferences. The app awakes the phone only when it is time to synchronize with the routers.
But if you notice battery issues with the app, you should either disable the Background Service (in the app preferences) or increase its frequency. In any case, please do let me know of that issue by sending a feedback via the app.



#### Modify or delete the contents of your USB storage / Read the contents of your USB storage
We use storage access to store your data on your device. For example, this permission is used in the following cases:
<ul>
<li>when you perform a "Backup" action via the app, the router settings are saved on your device, so you can share the resulting backup. Same thing when you perform a "Restore router" action via the app, where the backup file is read from your device.</li>
<li>usage data about hosts connected to your router is stored on your device on a regular basis, so that you have fast access to it.</li>
</ul>

