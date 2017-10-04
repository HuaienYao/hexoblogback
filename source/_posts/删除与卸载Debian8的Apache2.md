---
title: 删除与卸载Debian8的Apache2
date: 2017-09-18 21:28:16
tags: 
- 技术 
- VPS 
- 后端 
---

参考源：[Linux Tips][1]
由于某些主机提供商在重装系统后系统自带apache2，但是我又不需要，我需要nginx。如果不删除会导致冲突。
所以上网查询了下删除apache2的资料。
<!-- more -->

> Uninstall and Remove Apache2 on Debian 8
> 
> We are going to uninstall and remove Apache2 from our Debian system.
> 
> First we have to stop any running instance of Apache2, because Apache2
> will not be properly removed while it is running.
> 
> For stop Apache2 run below command …
> 
>     service apache2 stop
> 
> Now for remove Apache2 and pakchess run below command …
> 
>     apt-get purge apache2 apache2-utils apache2.2-bin apache2-common
> 
> then run below command …
> 
>     apt-get autoremove
> 
> Now finally, check if there is any configuration files or pages
> belonging to Apache2, which are still not removed…
> 
>     whereis apache2
> 
> example result like below …
> 
>     apache2: /usr/sbin/apache2 /usr/lib/apache2 /usr/share/apache2 /usr/share/man/man8/apache2.8.gz
> 
> Next if directory still exists the remove those manually …
> 
>     rm -rf /etc/apache2
> 
> Done … Great Job …
> 
> Some hosting provider installed Apache2 as default webserver so we can
> use this steps to uninstall Apache2 from our Debian system.

  [1]: https://ulinuxtips.com/uninstall-and-remove-apache2-on-debian-8/