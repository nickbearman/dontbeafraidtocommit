# How to report a bug

If and when you spot a problem with the software you're using, it's good practice to report this. As a non-expert coder it's a hugely useful way of contributing to a project.

However, there are right ways and wrong ways of reporting a bug!

##Specifically say what's wrong##

Get as much useful information into your initial communication about the problem as you can. The developer will need to reproduce your problem before he can try and fix it. If you simply say "It's broken" or "It crashed" then the only thing the developer will be able to do will email you back and ask for more information about the problem. Therefore provide the following information as a minimum:

 1. What exact version of the software are you using?
 2. What operating system are you using?
 3. (If appropriate) what installation method did you use?
 4. Exactly what steps did you take to trigger the bug?
 5. Is the problem reliably reproducible, eg does it happen each time you do the same steps?

##Explore different configurations##

If you're able, see if you can reproduce the problem on a different computer. Even better, try and reproduce it on a different operating system. If it's web-based, try different browsers. Ensure that you don't change too many variables at once though- it's important to test with the same version of the software.

Report the results of these tests to the developer. Let them know the configurations that didn't trigger the problem as well as the ones that did.

##Use the proper channels for researching and reporting the problem##

###Bug Trackers###

Most software projects have a dedicated bug tracker for reporting problems. This the correct place to report your problem rather than any other channel, such as twitter o email, even if it is quicker for you to dash off an email to someone, however quick and easy it is to do that. 

Firstly, check to see if the problem has been reported before. This could mean searching for closed issues as well as open ones. Most bug trackers have a method of filtering the issues to help with this.

*If you find your bug already reported, but you can provide more information on the problem, then add this to the discussion as it will help the developer solve it.*

###Mailing Lists###

If you're not sure it's a genuine bug, there's no harm in reporting it anyway. However if you're not keen on doing that, then the next channel to use is the project mailing list. Again report the same information as above to help people try to reproduce the problem.

##Providing an example##

If possible provide an exact example that demonstrates your problem. This could be a code snippet, a SQL query, or even a shape file or QGIS project. If the code is short, then you can use something like a [GitHub Gist](https://gist.github.com/) to share it. Otherwise attach your files to the bug report or mailing list message. If that's not possible then consider hosting the files somewhere online for people to download.

*Always create the Minimum Working Example (MWE) that demonstrates your problem. Remove anything that is unnecessary as this might introduce different problems or obscure the issue.*

##Be nice!##

**This problem may be causing you some trouble and making it hard for you to do your work, but being rude to the developer is not going to make him inclined to fix your issue.**

Your priorities are not the same as those of the developer. Do you have a work-around, such as using a different computer, or a different software package? If your problem is truly urgent and you have no work-arounds then consider hiring someone to fix the problem, or try to fix it yourself. Many open source projects do list companies that offer commercial support, so consider contacting them. 

The more information you can provide about your issue, the easier it will be for someone to fix it, and the more likely it is to happen.

##Software specifics##

###Web-based software###

Most modern browsers now come with some form of developer console and toolkit. Examples include:

 * [Chrome Developer tools](https://developer.chrome.com/devtools)
 * [Firebug for firefox](http://getfirebug.com/)
 * [Firefox Toolbox](https://developer.mozilla.org/en-US/docs/Tools/Tools_Toolbox)
 * [Internet Explorer F12 Developer tools](https://msdn.microsoft.com/en-us/library/gg589507(v=vs.85).aspx)

###QGIS###

**When reporting QGIS issues it's really important to provide information on the source of your installation. For windows users, did you use the stand-alone installer or OSGeo4W? For linux users which repository did your software come from?**

QGIS has a number of options for helping you debug problems including the messages panel, which logs messages for plugins as well as the main software itself. This can be activated from the bottom right corner of the main window in QGIS 2.14

![QGIS Message Panel](../images/qgis_messagepanel.png)

Lutra Consulting have also released a plugin that helps with the bug reporting process. It's a little tricky to set up and use but extremely useful. Find it on [plugins.qgis.org](http://plugins.qgis.org/plugins/report/) and instructions for use on their [blog](http://www.lutraconsulting.co.uk/blog/2016/05/12/qgis-report-plugin/).

See the online documentation [help pages](http://docs.qgis.org/2.8/en/docs/user_manual/preamble/help_and_support.html) for details of all the mailing lists and bug trackers.

QGIS maintains a list of companies offering commercial support- see [qgis.org/en/site/forusers/commercial_support.html](http://www.qgis.org/en/site/forusers/commercial_support.html) for details.



