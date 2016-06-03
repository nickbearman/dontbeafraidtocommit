#Ninja problem-solving, scripting and debugging##

A really good approach to running software on your computer, for both development and debugging purposes, is to consider creating sandboxed enviroments for each piece of software. This allows you to keep all the dependencies for the program packaged up with it, and isolated from other progams on your computer.

You can even use this approach to running multiple versions of software side by side.

There are a number of alternative approaches to this, some of which are more suited for certain types of software.

##Python##

Create a [virtual environment](http://docs.python-guide.org/en/latest/dev/virtualenvs/) to run the python program in. This is good practice anyway as it keeps all the dependencies for the program in one place, and separate from those used by other programs. 

*Virtual Environments can be tricky to install and set up on Windows. Try [this guide](http://www.tylerbutler.com/2012/05/how-to-install-python-pip-and-virtualenv-on-windows-with-powershell/).*

##Virtual Machines##

Virtual Machines are complete operating systems that run inside a "Guest" on your local computer (the host). You can download pre-built virtual machines, or build your own from an operating system iso file. This allows you, for instance, to run a linux guest on a windows host or vice versa.

[Virtualbox](https://www.virtualbox.org/) is the most common free virtualisation system. You can get a pre-configured Virtual Machine of the OSGeo Live Distribution from the [OSGeo Live site](http://live.osgeo.org/en/index.html).

Virtual Machines take up a lot of disk spaces and resources on your host computer, but do provide a completely separate environment to work in. You can, however, share files between the host and guest, and unlike a bootable DVD you can save the system state when you reboot.

##Docker##

A [Docker](https://www.docker.com/) "container" wraps up a piece of software in a complete filesystem. Unlike a Virtual Machine, it doesn't contain the whole operating system, but contains all the code, libraries, system tools and runtime that it needs.

> Virtual Machines are like houses, each with it's own infrastructure. Containers are like apartments, each shares the infrastructure using only what it needs

[http://sproke.blogspot.co.uk/2016/05/spatial-data-processing-with-docker.html](http://sproke.blogspot.co.uk/2016/05/spatial-data-processing-with-docker.html)

Some work has been done to get QGIS working in a Docker container, these are untested and included here for interest:

 * [docker-qgis-debian](https://bitbucket.org/timcera/docker-qgis-desktop-debian) - possibly cross-platform?
 * [qgis-desktop-in-docker](http://kartoza.com/qgis-desktop-in-docker/) - linux only?
 * [docker-qgis-orchestration](https://libraries.io/github/qgis/docker-qgis-orchestration) - for QGIS server?

