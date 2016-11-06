---
layout: page
title: "Prerequisites"
category: doc
date: 2015-05-21 23:21:39
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

Prior to starting using the app, you should make sure the following requirements are met:

<ol>
<li>The Router(s) you intend to use the app with runs a DD-WRT firmware</li>
<li>An SSH server is available and running on the Router(s)</li>
</ol>

### DD-WRT Firmware
Installing DD-WRT on your Router(s) is out of the scope of this guide. Please refer to the official <a href="http://www.dd-wrt.com/">DD-WRT Site</a> for instructions.

### SSH
Secure Shell, or SSH, is a command interface and protocol for securely getting access to a remote host. It has been chosen as the preferred secure communication channel between DD-WRT Companion and your DD-WRT Router.

#### Enabling SSH

From a computer, use a browser to login to the Web Management Interface of your Router, e.g.: http://192.168.1.1. 

Note: The app attempts to guess the IP Address of your Router(s), by fetching the gateway address of the network your phone is connected to. Just connect to a Wi-Fi network provided by the Router, and open the app on your Phone.

<div>
	<img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/7.1.0/add_new.png" width="280" height="563" alt="Tap on the Add Router Button"/>&nbsp; <img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/7.1.0/wizard_register_basic_details.png" width="280" height="563" alt="Potential IP Address of the Router"/>
</div>

<!-- 
![Tap on the Add Router Button](https://raw.githubusercontent.com/rm3l/ddwrt-companion/gh-pages/assets/7.1.0/add_new.png) &nbsp; ![Potential IP Address of the Router](https://raw.githubusercontent.com/rm3l/ddwrt-companion/gh-pages/assets/7.1.0/wizard_register_basic_details.png)
  -->

<br/>
Once on the Web Management Page of your Router, select the "Services" tab

![DD-WRT Web Interface - Services tab](http://apps.rm3l.org/apps/ddwrt-companion/assets/ddwrt_web_services_tab.png)

<br/>
Now scroll down to the "Secure Shell" settings, and make sure you have "SSHd" enabled, and either "Password Login" enabled (for password-based authentication) or "Authorized Keys" filled out (for public/private key authentication) , or both. 

The default port for SSH is 22, but it is recommended that you change it to a non-standard port above 1024 for security reasons. Remember the port you set, as you will need to enter it into your SSH client (and the DD-WRT Companion app) in order to connect to the router.

For example:

![DD-WRT Web Interface - Secure Shell](http://apps.rm3l.org/apps/ddwrt-companion/assets/ddwrt_web__secure_shell.png)

<br/>
Finish by scrolling down to the bottom of the page. Then click on "Save", then "Apply Settings", and "Reboot Router" buttons:

![DD-WRT Web Interface - Secure Shell](http://apps.rm3l.org/apps/ddwrt-companion/assets/ddwrt_web__save_apply_reboot_buttons.png)

##### Password method

If you have enabled the "Password Login" option in the "Secure Shell" settings, then you will need the following info to let DD-WRT Companion connect to the router:
<ul>
<li><u>User</u>: <b>root</b></li>
<li><u>Password</u>: the password you set in the web interface
</ul>

##### Public/private key

Public key authentication is one of the most secure methods of logging into SSH. It is considered as secured, as all transmissions are encrypted with a key that only the client and server will have.

To enable it, you will need to generate a Public/Private key pair on your desktop machine, then copy the public key in the router (actually, in the "Authorized Keys" text area of the "Secure Shell" settings).

On Windows, you can make use of <a href="http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html" target="_blank">Putty/PuttyGen</a> software.

On Linux or Mac OS X, make use of the <tt>ssh-keygen</tt> command-line tool, e.g.:

```bash
jedi:~ rm3l$ ssh-keygen -t rsa
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/rm3l/.ssh/id_rsa): /tmp/my_rsa_privkey    
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /tmp/my_rsa_privkey.
Your public key has been saved in /tmp/my_rsa_privkey.pub.
The key fingerprint is:
d1:8b:e8:29:bc:9e:31:ce:db:31:c9:94:d6:e5:35:51 rm3l@jedi.local
The key's randomart image is:
+--[ RSA 2048]----+
|            ..E  |
|         .   .   |
|        . o o    |
|       + = o .   |
|      = S o      |
|   . = o         |
|    = B          |
|   o B o         |
|   .B..          |
+-----------------+
jedi:~ rm3l$ 
```


![DD-WRT Web Interface - Secure Shell](http://apps.rm3l.org/apps/ddwrt-companion/assets/ddwrt_web__secure_shell__pubkey.png) 

<br/>
As the name implies, the public key is intended to be public, while the private key must be kept secret.

DD-WRT Companion actually behaves as an SSH Client, and as such, it will need the private key to authenticate against the router (which will in turn check it against the public keys you copied beforehand).

Of course, such sensitive information is encrypted once again locally, and never ever leaves your mobile device. 

#### Remote Access
By default, the SSH Server on some DD-WRT Routers may not accept incoming connections from external networks (such as the internet). Thus, you may not be able to remotely manage your routers with the app, unless connected to a WiFi network provided by the router.

To enable remote SSH access (see the screen capture below):
<ol>
<li>Head to the "Administration" tab and the "Management" sub-tab on the Web Interface</li>
<li>Enable "SSH Management" under the section titled "Remote Access"</li>
<li>Enter the same port number as specified in the section above (22 is the default SSH port). This opens the port in the firewall.</li>
<li>Click on "Save", then "Apply Settings", and "Reboot Router" buttons</li>
</ol>

![DD-WRT Web Interface - Remote SSH](http://apps.rm3l.org/apps/ddwrt-companion/assets/ddwrt_web__secure_shell__remote.png)

#### Testing the setup

As DD-WRT Companion assumes the Router has a fully working SSH server, we generally recommend you make sure you can manually connect to the Router from a computer, using the same credentials you intend to pass to the app.
If everything works as expected, then you should have no problem using the app with your Router.

##### Linux or Mac OS X

Open up a Terminal application. Depending on how you configured the Router "Secure Shell" settings, you may need any of the commands below.

###### Password-based login

Issue the following command, where <tt>ROUTER_IP_OR_DNS</tt> is the Router IP Address or DNS name. 

```bash
ssh -v -p 22 -l root ROUTER_IP_OR_DNS
```

At the password prompt, specify the password you set in the DD-WRT web interface (replace the port "22" accordingly if you specified something other than the default one):


###### Private-key based login

Issue the following command, where <tt>ROUTER_IP_OR_DNS</tt> is the Router IP Address or DNS name, and <tt>/path/to/my/private/key</tt> the absolute or relative path to your private key file. 

```bash
ssh -v -p 22 -l root -i /path/to/my/private/key ROUTER_IP_OR_DNS
```

If the private key requires a passphrase, you will be prompted to enter it. As always, replace the port "22" accordingly if you specified something other than the default one:


##### Windows

<a href="http://www.chiark.greenend.org.uk/~sgtatham/putty/" target="_blank">Putty</a> comes again to the rescue, to help test the setup.
