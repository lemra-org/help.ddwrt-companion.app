---
layout: default
title: "DD-WRT Companion"
order: 1
---

<!-- Begin Cookie Consent plugin by Silktide - http://silktide.com/cookieconsent -->
<script type="text/javascript">
    window.cookieconsent_options = {"message":"This website uses cookies to ensure you get the best experience on our website","dismiss":"Got it!","learnMore":"More info","link":null,"theme":"dark-top"};
</script>

<script>
  (function (w,i,d,g,e,t,s) {w[d] = w[d]||[];t= i.createElement(g);
    t.async=1;t.src=e;s=i.getElementsByTagName(g)[0];s.parentNode.insertBefore(t, s);
  })(window, document, '_gscq','script','//widgets.getsitecontrol.com/59849/script.js');
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

<div class="lead">DD-WRT Companion is a mobile app that lets you connect to, monitor and manage your DD-WRT routers on the go.</div>


[![Public Roadmap](https://img.shields.io/badge/Roadmap-vote%20for%20features-ff69b4.svg)](https://ddwrt-companion.app/roadmap)

### TL;DR
DD-WRT is a Linux based alternative OpenSource firmware suitable for a great variety of WLAN routers and embedded systems.
However, its web interface is quite impractical to navigate with from mobile devices.

This app aims at making DD-WRT devices management and monitoring a breeze, right from your mobile  device.

### Introduction
The overall rationale behind this project is to provide a set of apps dedicated to manage various routers and embedded devices with various firmwares. 

At this time, I am targeting DD-WRT routers, but the implementation aims at being flexible enough to support other firmwares (Tomato, OpenWRT, …) and their variants.

The app currently assumes the Router has a fully working SSH server (and, if required, external access if your router is behind a NAT network). 

It works with both private key and password based authentication methods.

### Supported Platforms

The following platforms are supported so far:

<ul>
 <li><a href="https://play.google.com/store/apps/details?id=org.rm3l.ddwrt" target="_blank">Android</a></li>
</ul>


### Supporting the project
If you find this project useful, you can help support further developments, by
<ul>
 <li>purchasing the premium full-featured and ad-free version of the app:
<br/>
<a href="https://play.google.com/store/apps/details?id=org.rm3l.ddwrt&utm_source=global_co&utm_medium=prtnr&utm_content=Mar2515&utm_campaign=PartBadge&pcampaignid=MKT-AC-global-none-all-co-pr-py-PartBadges-Oct1515-1" target="_blank"><img alt="Get it on Google Play" src="https://play.google.com/intl/en_us/badges/images/apps/en-play-badge-border.png"  width="260" height="85"/></a>
&nbsp; &nbsp;&nbsp;
<a href="http://www.amazon.com/Lemra-DD-WRT-Companion/dp/B00RN7HEI4" target="_blank">
<img src="https://images-na.ssl-images-amazon.com/images/G/01/AmazonMobileApps/amazon-apps-store-us-gray.png" alt="Available at Amazon AppStore" /></a> 
 </li>
</ul>

Also feel free to report any issue you might run into or any feature suggestion you might come up with. You can do so from within the app itself or by using the "Send Feedback" button in these pages.

### About

Should you have any questions or issue, please drop me a line at <a href="mailto:apps+ddwrt__web@rm3l.org?subject=About+DD-WRT+Companion+App">Armel Soro &lt;apps _AT_ rm3l _DOT_ org&gt;</a> or join me on <a href="https://twitter.com/DDWRT_Companion" target="_blank">twitter://@DDWRT_Companion</a>


