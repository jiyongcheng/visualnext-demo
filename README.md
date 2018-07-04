# visualnext-demo
1.修改 errors/local.xml.template to errors/local.xml
2.修改 app/etc/local.xml to app/etc/local.xml.bk, 这样可以重新安装
3.修改目录权限，在Dockerfile里面写
RUN chown -R www-data:www-data src/app/etc src/var src/media
RUN chmod -R go+rw src/app/etc src/var src/media
现在还没确定具体是哪一个命令管用
