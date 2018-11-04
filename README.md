# TUF

# フォルダ構成
./launch_apache_cent6/  ...Cent6上でapacheを自動インストール  
./launch_apache_cent7/  ...Cent7上でapacheを自動インストール  
./launch_nginx_cent7/   ...Cent7上でnginxを自動インストール  
./launch_nginx_cent6/   ...Cent6上でnginxを自動インストール  
./launch_squid_cent6/   ...Cent6上でsquidを自動インストール  
./launch_squid_cent7/   ...Cent7上でsquidを自動インストール  

# 別途準備するアイテム
* rpm  
    squid-3.5.16-1.el6.x86_64.rpm ... launch_squid_cent6用  
    https://rpmfind.net/linux/centos/7.5.1804/os/x86_64/Packages/squid-3.5.20-12.el7.x86_64.rpm  
* repo
    epel-httpd24.repo   ... launch_apache_cent6用
    https://repos.fedorapeople.org/repos/jkaluza/httpd24/epel-httpd24.repo  

# playbook配置後にやること
* 上記2つのファイルをダウンロードする
* 上記2つのplaybookの転送元ファイルのパスを書き換える
（要確認）/var/lib/jenkins/middle/...

# 残課題
* Cent7版のyum install 時のバージョン指定（latest -> present & xx-2.4）