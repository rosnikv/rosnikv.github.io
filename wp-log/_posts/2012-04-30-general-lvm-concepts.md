---
layout: post
category: Log
title: GENERAL LVM CONCEPTS
---

(Topic based on red hat linux) Logical Volume Management provides a more flexible way to manage disk space than physical disk partotions. 
Raw disk space in physical disk partitions can be pooled together or divided up into virtual partitions called logical volumes. 
This allows a number of powerful features,such as the ability to create file systems larger than any one disk,the ability to divide up asingle disk into more than fourteen file systems,and the ability to easily extend an existing file system with more space without the need to reformat it. 

*Implementation of LVM storage with command -Line Tools Prepare Physical Volume 

1. _fdisk_ is used to create a new partition for use with LVM.Always set the type to 0X8e Linux LVM on partition to be used with LVM. Alternatively you can use a whole disk,a RAID array,or a SAN disk. 

2. _pvcreate  /dev/vdaN_ is used to initialize the parttion for use with LVM as a Physical Volume. 

*Creating a Volume Group 

1. _vgcreate vgname /dev/vdaN _ will create a volume group named vgname made up of the physical volume /dev/vdaN you can add new physical volume later with _vgextend_. 

*Create and Use a New Logical Volume 

1. l_vcreate  -n lvname  -L  2G  vgname  _creates a new 2GB logical volume named lvname from the available physical extends on vgname. 

2. mkfs -t ext4 /dev/vgname/lvname will create an ext4 file system on the new logical volume. 

3. _mkdir /data _makes directory needed as a mount point. 

4. Add an entry to the _.etc/fstab _file: _/dev/mapper/vgname-lvname   /data  ext4   defaults  1  2_ 

5. Run _mount  -a _to mount all the file systems in /etc/fstab , including the entry you just added.

*link: https://rosnikv92.wordpress.com/2012/04/30/general-lvm-concepts/
author: rosnikv
description: 
post_id: 29
created: 2012/04/30 18:34:28
created_gmt: 2012/04/30 18:34:28
comment_status: open
post_name: general-lvm-concepts
status: publish
post_type: post*
