#mysql远程访问
*   初次安装mysql成功后由于权限问题一般从远程是无法直接访问mysql服务的；
*   可通过在安装mysql服务的主机上登录mysql，然后在“mysql”库的“user”表中增加允许远程访问的配置；
*   在“user”表中将已有的root用户信息的“host”字段（原来的值一般为“localhost”）更新为“%”，以一种通配符的方式重新进行设置；

*   最后记得执行命令`flush privileges;`
    
