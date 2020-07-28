# Angular-网易云
    +Thanks to the original author's teaching, I benefited a lot.
    
    +Thanks for the open source data provided by the interface provider to facilitate our learners to use it.
    
    +TIPS:When it comes to security issues, it is not recommended to deploy the project to the server to prevent privacy issues.

## 启动接口（网易云音乐接口）：
    git clone https://github.com/Binaryify/NeteaseCloudMusicApi.git
    
    npm install
    
    npm start

## 启动项目：
    git clone https://github.com/lycHub/ng-wyy.git
    
    npm install
    
    npm start

## angular 模块化思想
    +Use Appmodule to manage the Coremodule;

    +Coremodule: As the root module for myself,other module only to put them in this module.It convienent for us to maintian modules;

    +sharemodule: Put the generic component,module in it,other module can use it;

    +servicesmodule: Put all services module in it;

    +pagesmodule Put all pages in it(/home/login/rigister...)

    +Modular design is recommended by Angular.io,This makes the project more clear and easy to maintain and manage；

## 项目中的小坑
    +angular关于params 分页中的queryString应使用node 中的const queryString = require('query-string');
    若使用ECMA标准的import {queryString} from 'query-string';会报错没有导出类

    +命名要简洁，易懂，且拼写检查要及时进行，否则会出现意外

    +ng : 无法加载文件 C:\Users\kkwang\AppData\Roaming\npm\ng.ps1。未对文件 C:\Users\kkwang\AppData\Roaming\npm\ng.ps1 进行数字签名。无法在当前系统上运行该脚本。有关运行脚本和设置执
    行策略的详细信息，请参阅 https:/go.microsoft.com/fwlink/?LinkID=135170 中的 about_Execution_Policies。
    所在位置
    set-ExecutionPolicy RemoteSigned

    +更改权限为A
    get-ExecutionPolicy
    显示： RemoteSigned 已完成错误更改"# Angular-wyMuxic" 
