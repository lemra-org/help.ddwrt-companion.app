---
layout: page
title: "Usage"
category: tasker
date: 2017-05-13 16:33:07
order: 2
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

To use <a href="https://play.google.com/store/apps/details?id=org.rm3l.ddwrt.tasker">DD-WRT Companion Tasker Plugin</a>, open Tasker (or the appropriate automation app that supports Tasker plugins), and DD-WRT Companion will appear as an Action Plugin.

### Tasker

<ol>

<li>Open Tasker. Then switch to the "Tasks" tab. Edit existing tasks, or create a new one. In the "Task Edit" window, you will be able to add an Action by clicking on the '+' symbol.

<div>
	<img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/1-open-tasker.png" width="280" height="563" alt="Open Tasker and click on the 'Tasks' tab"/>&nbsp; <img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/2-task-edit.png" width="280" height="563" alt="Edit Task actions"/>&nbsp; <img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/3-task-edit-select-action.png" width="280" height="563" alt="Edit Task actions"/>
</div>
<br/>
<br/>
</li>

<li>On the 'Select Action Category' dialog, click on 'Plugin' and select DD-WRT Companion Tasker plugin. Now click on the 'Pencil' to edit the Plugin configuration for this Action.
Select the appropriate router and command to send out, and fill in the proper parameters as needed. Do <b>not</b> forget to <b>save</b> your configuration.

<div>
	<img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/3-task-edit-select-action-plugin.png" width="280" height="563" alt="Click Plugins"/>&nbsp; <img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/4-action-edit.png" width="280" height="563" alt="Select DD-WRT Companion Tasker plugin"/>&nbsp; <img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/5-tasker-plugin-configuration.png" width="280" height="563" alt="Edit Plugin Configuration"/>
</div>
<br/>
<br/>
</li>

<li>Once validated, you will see a confirmation of some of the settings. You can return back to Tasker tasks. 

<div>
	<img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/5-tasker-plugin-configuration-validated.png" width="280" height="563" alt="Plugin configuration saved"/>&nbsp; <img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/6-task-edit-with-actions.png" width="280" height="563" alt="View all actions in task"/>
</div>
At this stage, you can manually test the configuration by executing the Action (click on the '>' button).
<br/>
<br/>
</li>

<li>You can now return to the Tasker main window. At this point, to benefit from automation, you may want to create a 'Context', which will automagically trigger the execution of the task(s) you defined earlier. For that, you can slide to the 'Profiles' tab and create a new Profile (link between Contexts and tasks that should run when the conditions are met).

For example:

<div>
	<img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/7-tasker-with-test-task.png" width="280" height="563" alt="Task added to Tasker"/>&nbsp; <img src="https://raw.githubusercontent.com/rm3l/help.ddwrt-companion.rm3l.org/master/assets/tasker/10-example-profile.png" width="280" height="563" alt="Sample profile"/>
</div>
<br/>
<br/>
</li>

</ol>


