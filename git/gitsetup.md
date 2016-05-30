# First time setup steps

Since Git is designed to record changes to a global repository, it needs to be able to identify you and provide a means of contact. When you first start working with Git, you need to do a couple of initial setup steps to configure this information.

These steps are global, in that they will apply for all repositories you set up on your current local machine.

**This information will be visible in all repositories you make public so don't use details you'd rather keep private**

*These settings can be overridden on a per-repository basis but we won't cover that here*

At your git terminal type:

	git config --global user.name "Your name"
	git config --global user.email "your.email@yourmailserver.com"

The command:

	git config --list

will show you the existing Git config settings.

There are many additional settings that can be configured using git-config. For a comprehensive listing see [git-config](https://git-scm.com/docs/git-config).

## Configuring Git to use the text editor of your choice

By default Git will use your operating system's default editor. On Windows that's probably NotePad, on Mac it's probably Text Edit. On Linux- vi, or nano. The following command is used to set the default text editor for Git:

	git config --global core.editor "/path/to/your/editorexecutable"
 	
The exact format of the path to use here will be dependent on your operating system. [This link](http://swcarpentry.github.io/git-novice/02-setup.html) shows you how to set up the core editor config for a number of example packages in Windows, Mac and Linux.