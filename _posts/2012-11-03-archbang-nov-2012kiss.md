---
title: ArchBang nov 2012:KISS
link: https://rosnikv92.wordpress.com/2012/11/03/archbang-nov-2012kiss/
author: rosnikv
description: 
post_id: 123
created: 2012/11/03 06:29:54
created_gmt: 2012/11/03 06:29:54
comment_status: open
post_name: archbang-nov-2012kiss
status: publish
post_type: post
---
# ArchBang nov 2012:KISS

**ArchBang nov 2012:KISS(Keep it Simple Stupid)!** Latest archbang(released on november) **more user-friendly,simple,fast and stable**..after small config... For simple installation this link will help you: <http://archvortex.blogspot.in/2011/09/simple-archbang-installation-guide.html> 

![](http://rosnikv92.files.wordpress.com/2012/11/2012-11-03-1351901710_1366x768_scrot.png?w=300) 

Arch Linux defines simplicity as _without unnecessary additions, modifications, or complications_, and provides a lightweight UNIX-like base structure that allows an individual user to shape the system according to their own needs. In short: an elegant, minimalist approach.*

**Complexity without complication.

**Simplicity of _implementation_, code-elegance, and minimalism shall always remain the reigning priorities of Arch development.

**Arch Linux targets and accommodates competent GNU/Linux users by giving them complete control and _responsibility_ over the system.

Arch Linux uses simple tools, that are selected or built with openness of the sources and their output in mind. 
By keeping the system simple, Arch Linux provides the freedom to make any choice about the system.
Some changes for this release:
\- QDarkStudio4 default GTK theme
\- Shotwell picture viewer 
\- Improved Conky 
\- Epdfview replaces zathura 
\- simple clean tint2 panel 
\- Broadcom wireless added 
\- virtualbox-archlinux-additions
\- Mobile Broadband modem capability added to Network Manager 

![](http://rosnikv92.files.wordpress.com/2012/11/2012-11-04-1352012943_1366x768_scrot.png?w=300) 

You can embed the lxterminal in desktop using this link <http://bbs.archbang.org/viewtopic.php?pid=1714> you can change your conky like above using this script:

```
//SCRIPT BEGINS 
>background yes 
use_xft yes 
xftfont monospace:size=9 
xftalpha 1 
update_interval 1.0 
total_run_times 0 
own_window yes 
>own_window_transparent yes own_window_type desktop own_window_hints undecorated,below,sticky,skip_taskbar,skip_pager >own_window_colour black double_buffer yes minimum_size 1 1 maximum_width 240 draw_shades no draw_outline no draw_borders no >draw_graph_borders no default_color gray default_shade_color 000000 default_outline_color d9d7d6 alignment tr gap_x 12 gap_y >12 no_buffers yes uppercase no cpu_avg_samples 2 override_utf8_locale no color1 red color2 gray 
```

############################################## #  Output ############################################## 
```
TEXT ${image $HOME/archlinux2inverted.png -p 9,10 -s 250x200} 
${font Comfortaa:bold:size=13}
${offset 200}
${time %A} 
${color #66cd00}
${font Comfortaa:bold:size=36}
${time %H}
${font}${color #7fff00}
${font Comfortaa:bold:size=28}
${voffset -27}${time :%M:%S}${font} 
${font Comfortaa:bold:size=8}
${offset 100}${time %d %b %Y} 
${color #ffd700}CPU: 
$alignr${cpu cpu0}% ${cpubar cpu0} RAM: $alignr$mem/$memmax $membar ${color #008b00} 
${font sans-serif:bold:size=8}SYSTEM ${hr 2} Hostname: $alignr${color1}$nodename${color #008b00} Kernel: $alignr${color1}$kernel${color #008b00} Arch:${alignr}${color1}$machine${color #008b00}
Processes: ${alignr}${color1}$processes ($running_processes running)${color #008b00} 
Uptime: ${alignr}${color1}$uptime${color #008b00}
Load: ${alignr}${color1}$loadavg${color #008b00} ${color #008b00}${font sans-serif:bold:size=8}TOP PROCESSES ${hr 2}
${font sans-serif:normal:size=8}${top_mem name 1}${alignr}${top mem 1} % ${top_mem name 2}${alignr}${top mem 2} % $font${top_mem name 3}${alignr}${top mem 3} % $font${top_mem name 4}${alignr}${top mem 4} 
% ${color #008b00}${font sans-serif:bold:size=8}SHORTCUT KEYS ${hr 2} ${font sans-serif:normal:size=8}Alt+F2$alignr 
Run Dialog Alt+F3$alignr Dmenu Super+space$alignr Main Menu Super+t$alignr Terminal Super+f$alignr File Manager Super+e$alignr Editor Super+m$alignr Media Player Super+w$alignr Web Browser Super+q$alignr Force Quit Super+g$alignr Character Map Super+l$alignr Lock Super+r$alignr Read the DOC Super+x$alignr Tiling Keybinds ${image ~/alogo.png -p 0,0 -s 190x45} ${color}
ACPI Battery: ${color DeepSkyBlue}$battery ${battery_bar 11,0} 
//END OF THE SCRIPT 
```
Note:The image you are going to use should be in Home directory. Fore more information go to :<http://wiki.archbang.org/index.php?title=Main_Page>

## Comments

**[Raghav](#25 "2012-12-03 07:26:00"):** good post....
