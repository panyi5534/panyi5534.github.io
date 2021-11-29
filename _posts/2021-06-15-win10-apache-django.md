---
layout: post
author: ted
---
win10 apache django

apache: <http://httpd.apache.org/docs/current/platform/windows.html#down>
D:\Apache24\conf>vim httpd.conf
```
Define SRVROOT "D:\Apache24"
```
<https://visualstudio.microsoft.com/visual-cpp-build-tools/>
<https://github.com/traviscross/apr/blob/master/include/apr_perms_set.h>
D:\Apache24\include\apr_perms_set.h  
C:\Users\Dell>set “MOD_WSGI_APACHE_ROOTDIR=D:\Apache24”  
C:\Users\Dell>pip install mod-wsgi  
<https://docs.djangoproject.com/zh-hans/3.2/howto/deployment/wsgi/modwsgi/>
C:\Users\Dell>mod_wsgi-express module-config  
E:\>django-admin startproject website  
E:website\>django-admin startapp backend  
D:\Apache24\conf>vim httpd.conf
```
LoadFile "d:/python/python39/python39.dll"
LoadModule wsgi_module "d:/python/python39/lib/site-packages/mod_wsgi/server/mod_wsgi.cp39-win_amd64.pyd"
WSGIPythonHome "d:/python/python39"

WSGIScriptAlias / "e:/website/website/wsgi.py"
WSGIPythonPath "e:/website"

Alias /static "e:/website/static"
<Directory "e:/website/static">
    AllowOverride None
    Options None
    Require all granted
</Directory>
```
D:\Apache24\bin>httpd.exe -k install  
D:\Apache24\bin>sc delete Apache24
