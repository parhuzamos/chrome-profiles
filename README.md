chrome-profiles v0.3
====================
  
**A quick&important note: currently there is no error checking, no setup, no configuration. It just works.**

What is this?
-------------

Google Chrome Profile selector/launcher and creator. You can create separate profiles in Google Chrome for every job/task/feature you work on.  
Each profile will have a different set of windows and tabs, cookies, login sessions and everything, just like "Incognito Window" but storing everything persistently. Each profile is a different process, so killing one process keeps the others running.  
If you quit the a profile (Ctrl+Shift+Q) its windows and tabs are closed but restored if you relaunch that profile. Make sure it's set so in Google Chrome settings.


Example
-------

Suppose you get a ticket to work on, let's call it "ticket-2001". You start "chrome-profiles" and create a new profile: "ticket-2001". A new Google Chrome window is opened.  
You navigate and login to the ticket managing system, open that ticket. That's one tab.  
You open a new tab, to see the feature on the live site. Tab two.  
A nother tab is for your local development environment to see your work in progress.  
You start working, creating login sessions, cookies, ...

Suddenly, a colleague asks if a nother feature has this and that. What now? Just start "chrome-profiles" and select that ticket/feature: "ticket-1234" that you previously worked on. All those windows, tabs, login sessions will be restored and you can pick up the work where you've left off.

Also, you can have multiple login sessions for the same site in different profiles. You can be logged in with many facebook users in the very same time and your sessions will be preserved after closing the process unlike in "Incognito mode". 

NOTE: if you want to close a profile, don't just close the windows. Make sure you exit Google Chrome with Ctrl+Shift+Q.


Tips
----

* Assign a global keyboard shortcut to "chrome-profiles". For me it's "Win+G". This speeds up starting different profiles.
* Again: close/leave a profile with Ctrl+Shift+Q!
* [Session Buddy](https://chrome.google.com/webstore/detail/session-buddy/edacconmaakjimmfgnblocblbcdcpbko?hl=en) - saves window, tab history and session
* [The Great Suspender](https://chrome.google.com/webstore/detail/the-great-suspender/klbibkeccnjlkjkiokjodocebajanakg) - "suspends" unused tabs after a configure amount of time

TODO
----

* Write some notes about the skeleton/base directory
* Implement creation of skeleton directory from the current config
* Profile directory configuration

Environment
-----------

Currently Linux. But it could be ported easily to other platforms.

Dependecies
-----------

* [zenity](https://help.gnome.org/users/zenity/stable/) - to provide GUI for selection and text entry  
    Install it with your favourite package manager.  
    For Ubuntu:
        sudo apt-get install zenity

        
...
---

If you made this far, buy me a drink:
[![Fund me on Gittip](https://s3-eu-west-1.amazonaws.com/com.parhuzamos/adblogga/gittip-logo.png)](https://www.gittip.com/parhuzamos/)
