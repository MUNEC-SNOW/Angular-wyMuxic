# Angular-网易云
    感谢原作者的教学，使我受益匪浅
## angular 模块化思想
    appmodule 管理单独coremodule

    coremodule 相当于自己的根模块将其他模块导入至此

    sharemodule 把一些公共的样式，组件，指令导入导出，方便其他特性模块引用这些组件

    servicesmodule 所有的服务放入此

    pagesmodule 管理所有的页面（主页/登录/..）

    模块化设计符合推荐设计模式，方便日后管理

## 项目中的小坑
    angular关于params 分页中的queryString应使用node 中的const queryString = require('query-string');
    若使用ECMA标准的import {queryString} from 'query-string';会报错没有导出类

    命名要简洁，易懂，且拼写检查要及时进行，否则会出现意外

    ng : 无法加载文件 C:\Users\kkwang\AppData\Roaming\npm\ng.ps1。未对文件 C:\Users\kkwang\AppData\Roaming\npm\ng.ps1 进行数字签名。无法在当前系统上运行该脚本。有关运行脚本和设置执
    行策略的详细信息，请参阅 https:/go.microsoft.com/fwlink/?LinkID=135170 中的 about_Execution_Policies。
    所在位置

    set-ExecutionPolicy RemoteSigned

    更改权限为A
    get-ExecutionPolicy
    显示： RemoteSigned 已完成错误更改"# Angular-wyMuxic" 
