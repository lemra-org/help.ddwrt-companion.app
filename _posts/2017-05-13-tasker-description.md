---
layout: page
title: "Description"
category: tasker
date: 2017-05-13 16:31:48
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

<div class="lead"><a href="https://play.google.com/store/apps/details?id=org.rm3l.ddwrt.tasker">DD-WRT Companion Tasker Plugin</a> is a Tasker Action Plugin that allows you to automate the act of launching commands on remote routers registered in DD-WRT Companion app</div>

<a href="http://tasker.dinglisch.net/">Tasker</a> is a powerful application for Android which allows to perform tasks based on contexts (application, time, date, location, event, gesture) in user-defined profiles, clickable or timer home screen widgets.
Tasks can be executed either manually or automatically.

Below is a simple overview of some of Tasker concepts:
<ul>
<li><b>Action</b> &mdash; The basic element of Tasker. It refers to phone or tablet functions and features that perform something or brings the phone to a certain state. Tasker supports hundreds of actions, and external plugins (such as DD-WRT Companion Tasker Plugin) can provide additional actions.</li>
<li><b>Task</b> &mdash; A group of actions. Usually linked to a trigger or "context", but can also be a free-floating, standalone task executed manually.</li>
<li><b>Context</b> &mdash; Situations or conditions which, when true, trigger the execution of the task(s) associated with it. An incoming notification, the opening of an app, or connecting to a certain WiFi network are all examples of contexts which can be used to trigger a task</li>
<li><b>Profile</b> &mdash; Some sort of "container" or "package" for context(s) and linked task(s). You can define several contexts for a single profile, and all those conditions must be true for the linked tasks to run.</li>
<li><b>Variable</b> &mdash; A name for an unknown value that can change over time, like the battery level or the date.</li>
<li><b>Scene</b> &mdash; A custom-made user interface. You can create your own layout of buttons, menus, popups, and other UI elements.</li>
<li><b>Project</b> &mdash; A group of profiles, tasks, scenes, and variables.</li>
</ul>


DD-WRT Companion Tasker Plugin is available as a separate app to download <b>for free</b>.

It can be seen as an Action Plugin, in that it provides a set of actions that can be triggerred (either manually, or when certain events occur).

Note that this plugin should also work with other automation apps that support Tasker plugins, such as Automate.

As <b>security matters</b>, this plugin works in conjunction with DD-WRT Companion PIN protection and third-party integration features.

You can perform actions from a set of pre-defined commands, or optionally provide your own commands. 

Possible actions include (but are not limited to):

<ul>
<li>Reboot</li>
<li>Wake On LAN (WOL)</li>
<li>Toggle Internet Access Restriction Policies</li>
<li>Toggle WAN Access for a particular device</li>
<li>Toggle WOLd (Wake On LAN Daemon)</li>
<li>Toggle OpenVPN Client and Server statuses</li>
<li>Toggle PPTP Client and Server statuses</li>
<li>Clear ARP Cache</li>
<li>Clear DNS Cache</li>
<li>DHCP Release / Renew</li>
<li>Erase WAN Traffic Data</li>
<li>Stop / Start / Restart HTTPd (HTTP Server)</li>
<li>Reset Bandwidth Counters</li>
<li>Toggle Syslog</li>
<li>Provide your own custom command(s)</li>
<li>More to come in future releases...</li>
</ul>

This list may change in the future, as we keep enriching the app with additional capabilities.

Furthermore, to allow for better transparency, you have access to a detailed audit log of all actions performed via this plugin.
