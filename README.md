# ms
一个用python开发的新闻/评论微系统，各服务封装在docker中交付。
以下是个服务模块：  

1. 用户服务 
2. 新闻服务  
3. 评论服务   
```
以上三个微服务以flask开发，输出restful接口
```
4. kong：API网关
5. postgre  API网关要用到  
6. MariaDB  
7. redis  
8. nginx：    
    后台管理，用vue admin template框架
9. node js   
    前台页面的后端渲染，用vue实现
10. elastic search   
将新闻导入es，实现全文检索  
将nginx及各微服务的日志通过file beat导入进行分析  
制定各类规则，触发规则发钉钉进行预警
11. kibana
elastic search的UI界面
12. nifi  
一个数据转换工具。通过nifi将数据从mysql导入elastic search。
13. jenkins  
自动化测试及部署


