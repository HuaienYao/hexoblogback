---
title: 获取Windows Live Skydrive 唯一外链地址
id: 116
date: 2010-11-23 16:09:23
tags:
---

[CODE]javascript:var%20n=document.title.replace('%20-%20Windows%20Live','');var%20id=((location.hash=='')?window.selfPageData.currentItemHash:location.hash).replace('#resId/','');var%20u='http://storage.live.com/items/'+id+'?filename='+encodeURI(n);var%20p='http://'+document.location.host+'/redir.aspx?page=self&resId='+id;var%20e='<input%20onmouseover=%22this.select();%22%20onclick=%22this.select();%22%20value=%22';var%20f='%22%20style=%22width:580px%22%20type=%22text%22%20/>
';var%20d='by%20([Rpsh](%22http://rpsh.net/%22))';var%20c='\u5916\u94FE\u5730\u5740:'+d+e+u+f+'\u5206\u4EAB\u5730\u5740:'+e+p+f;var%20a=document.getElementById('content');var%20g=(a.getElementsByTagName('p')[0]);var%20b=g?g:document.createElement('P');b.innerHTML=c;a.insertBefore(b,a.firstChild);void(0)[/CODE] 