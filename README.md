简洁的云笔记本，支持加密，只读分享


# 环境和依赖

- 免数据库，直接放置于支持PHP5.3+的空间即可

- Apache和Kangle服务器使用.htaccess文件支持URL重写

- Ngnix使用ngnix.conf文件支持URL重写,需要将里面的代码复制到vps的伪静态里面

# 安装指南

- 检查并确认关闭 php.ini 设置里的magic_quotes_gpc设置为Off否则会导致保持HTML选项时自动增加\字符
- 解压全部文件到域名根目录即可，例如http://域名/
- 如要使用二级目录例如http://域名/二级目录/，则需要修改index.php文件。将目录设为固定的 $URL = "http://主域名/二级目录";
- 解压缩后需要新建一个目录，目录名称为"_tmp"注意，实际文件夹不含引号，并将此文件夹设置为777权限，否则文件无法保存，无法加密

# 友情提醒

文档设置密码之后只针对网页前端有保护作用，后端文件明码保存在_tmp文件中可直接编辑查看
因此不建议将重要资料保存在他人搭建的系统当中
