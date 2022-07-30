---
layout: post
category: Log
title: Virtual environments, Play safe in small Python Projects !
---

Creating virtual environment for small projects(python)  was new information for me.

This allows you to work on a specific project without worry of affecting other projects.

Let us check how to set up this.

Install pip or easy_install (easy_install and pip are python package installers that will make your life a lot easier when developing in python)
```
sudo yum install python-pip``
```
 Virtualenv is a tool to create isolated Python environments.
```
sudo pip install virtualenv virtualenvwrapper
```

Make a directory to store your virtual environments(depends on your project number :) )
```
mkdir virtual_env
```

Create a virtual environment
```
virtualenv virtual_env/virt1
```
To start using the virtual environment , you need to activate it.
```
source virtual_env/virt1/bin/activate
```
If  you are done with it, you can close it using command
```
deactivate
```
To delete a virtual environment, just delete its folder.

To install packages /modules, you can direct installation to the specific environment for  corresponding project. For example
```
 ~/virtual_env/virt1/bin/pip install requests

 ~/virtual_env/virt1/bin/pip install Django
```
These steps are with virtualenv . When you have a lot of virtual environments and it is difficult to handle , virtualenvwrapper will help. Install it using your favourite package installer.

Make sure you installed virtualenvwrapper already
```
source /usr/local/bin/virtualenvwrapper.sh
```
Create a virtual environment using virtualenvwrapper
```
mkvirtualenv virt1
```
This create a virt1 directory in current path.

To work with it:
```
workon virt1
```
This will deactivate the environment you are currently in.

 We can use _deactivate_ command here also.

Virtualenvwrapper provides some useful commands to deal with these environments like,

To remove :
```
rmvirtualenv virt1
```
To list  :
```
lsvirtualenv virt1
```
Explore more commands [here](http://virtualenvwrapper.readthedocs.org/en/latest/command_ref.html#managing-environments)

Happy Coding !!!


*link: https://rosnikv92.wordpress.com/2013/09/19/play-safe-using-virtual-environments/
author: rosnikv
description: 
post_id: 248
created: 2013/09/19 14:15:06
created_gmt: 2013/09/19 14:15:06
comment_status: open
post_name: play-safe-using-virtual-environments
status: publish
post_type: post*

## Comments

**[Soorej Kv](#28 "2014-01-05 13:52:11"):** happy coding

