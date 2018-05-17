# YLUI

## 前言

### YLUI是什么

YLUI是一款纯前端框架，是对WEB桌面UI的一个大胆尝试。

它凝聚了作者近一年的心血，作为[WIN10UI](http://win10ui.yuri2.cn)开源项目的升级版，承载了作者对WEB桌面设计风格的追求。

在前端技术日新月异的背景下，YLUI力图提供一种新的web应用组织形式。

如果你正在寻找一个漂亮的UI组件库，你应该选择bootstrap,layui,element-ui等项目。而你想要让这些应用建立联系，构成组织，并提供一个统一的门户，那么YLUI将会是一个不错的选择。

> YLUI提供的是应用组织框架，而不是应用开发工具，更不要因为它长得像浏览器就把它当浏览器使用，毕竟我们已经有太多浏览器可供选择了，不是吗？

> 注意，这不是一个免费软件，请仔细阅读版权声明信息`Lisense.txt`
### 特色

* 纯前端实现，高兼容性
* 延续windows界面操作逻辑，普通用户上手难度较低
* 简单直观的多APP管理，像桌面程序一样呈现你的web应用
* 统一的APP交互模型，保持各APP之间的独立性，降低子系统耦合度，支持跨域的APP通信
* 完美复刻桌面操作系统的菜单、磁贴、通知元素，良好的视觉表现力
* 兼容PC、平板电脑、手机等各大主流分辨率
* 可视化开发，降低开发者的学习难度
* 基于VUE.JS开发，支持数据序列化（可配置化），方便与后台做数据存取接口
* 详尽的开发文档

### 推荐使用场景

1. 个人云桌面
2. 企业办公平台
3. 云盘类应用
4. 中大型管理信息系统
5. 导航门户网站
6. H5打包应用
7. web开发工程师个人工具集

### 版本
2.0.2

### 相关链接

[YLUI官网](https://ylui.yuri2.cn) | [码外社区](http://www.bycodes.net/) | [官方交流群](https://jq.qq.com/?_wv=1027&k=5fAsios)

------------------------------------
## 开发记录

### TODO

* nwjs版
* APP STORE
* 声音
* IOS iframe的问题 -webkit-overflow-scrolling:touch
* skin字段
* 文档
* APP STORE
* 标题按钮组缩放bug
* 清理非必须代码
* 二级菜单在底部开启时表现不佳
* 关于界面，分离YLUI的介绍
* 合并小文件
* 菜单项文字溢出

### 日志
* 180517 2.0.2 修复图标组不能解散的bug；修改英文菜单溢出的bug（litins）
* 180514 删除demo APP；添加社区版的提示信息；
* 180430 细节优化，冗余清理;优化child的api；关于界面，分离YLUI的介绍；
* 180429 更正拼写错误 resizeable => resizable
* 180416 有缓存的情况下，省去启动画面；删去了jsonp请求，所有服务转入yl-server(未完成)
* 180412 优化app管理页面；新增APP属性version以及对应app函数getAppVersion
* 180411 新增dataCenter配置（是否展示数据管理）；添加数据格式不正确提示（ｅ啲缌唸提出）
* 180409 修复了_baseData返回不正确的bug;添加了信任APP eval的方法。
* 180406 修复了菜单打不开的bug;优化右键菜单css
* 180403 添加了一个日历插件；修复了卸载时依赖清除有残余的bug
* 180402 css微调，更多阴影；
* 180330 微调窗体阴影，取消边框；
* 180329 微调任务栏css;添加app动态壁纸;添加应用商店app安装模板;窗体位置以iframe为准;basic存档添加了一个纯黑壁纸；默认onload支持从load参数读取存档；
* 180328 窗体右键菜单显示尺寸位置;自动打开的应用没有source（关于“记住位置”功能）;打开菜单时隐藏桌面图标;
* 180327 引入了4个纤细的图标
* 180322 YL.init自动对数据格式化，参数省略时尝试读取ls（ylui-storage）;
* 180321 修复了IIS下xhr请求400的错误;修复了端口号不为80时丢失端口的bug; 移除错误回报机制；
* 180320 前缀统一为YL;修复了改前缀引起的一些bug；
* 180319 APP STORE雏形
* 180316 移除system的app store ，转为独立页面处理（yl-app-store，未完成）
* 180314 优化消息栏清空逻辑；不默认读取云存档；去除内嵌式应用商店框架；移除hbuilder工程代码（hbuilder打包需要mui配合）
* 180313 配合ylui.yuri2.cn完成后端demo;
* 180312 移除localStorage和loadsaveurl，统一由子页实现。
* 180309 安装接口加入依赖检测;磁贴也加入了角标;锁定应用将不可被卸载、覆盖修改;简化 sideBar btns;为第三方接口添加完成提示；
* 180308 删除信任体系；删除app回调体系;slider更正为sidebar;修复了卸载时侧边栏依赖bug；为第三方网站提供安装/卸载app的功能，更方便提供服务。为第三方网站提供setAppBadge设置徽标。
* 180307 添加官方APP浏览器;优化css；自动语言支持（默认英文，识别中文请求）;
* 180306 多语言支持完成;修正了jsonp的bug；防止图标重复打开（时间锁）
* 180305 部分国际化;手机自动低特效（可配置）;微调小图标css;完成子窗口安全重构，添加了同源检测和身份检测,发送源字段统一为from,添加close函数；
* 180302 部分完成子窗口安全重构;窗口可拖动;窗口的定位方式可选左对齐和顶部对齐了
* 180228 支持触屏拖动图标;优化右键菜单的css；
* 180227 一些设置转移到configs.js;lockApps机制;在线验证记录机制的雏形；
* 180226 winID更随机；全屏应用隐藏还原按钮；更多常量定义；新增官网ylui.yuri2.cn
* 180224 常量定义的软件名;在YL.static下添加了一些常量;优化css;大改图标逻辑代码，改为线性排列，更好的拖拽和排序效果
* 180223 添加了一个新的时钟插件；
* 180214 修复了一些浏览器卡在loading界面的bug；body背景设置为黑色，用于更顺眼的过渡；微调css;优化子窗口支持js
* 180211 修复了卸载产生的依赖性bug；新增很多菜单图标；打开方式新增“外部窗口”；
* 180209 窗口打开封面;优化快捷设置表单行为;磁贴支持按分组添加;子窗口token由可选变为默认；去除了刷新的图片动画；新建app的url过滤token；
* 180206 优化了一些css;修复了磁贴轻微拖拽误打开的bug;磁贴iframe现在带randomToken来保证最新；yl-system页面由hash传参改为post data传参
* 180205 磁贴可设置url自定义展示；修复磁贴点击和拖动事件的冲突；磁贴的也支持发送到、打开等功能了；手机浏览壁纸样式修正防止失真；
* 180201 微调drawer样式;win.childSupport表示子页是否加载了高级支持，并在地址栏做对应的微调;
* 180131 小菜单支持二级，优化右键菜单;磁贴列数固定为6;
* 180126 更好的响应式;slider.btns由对象改为数组
* 180125 可分组的磁贴，更好的响应式支持,使用了弹性盒使布局更紧凑;弹框样式优化；
* 180124 图标样式微调（减肥）;更丰富的右键菜单；可添加的侧边栏；菜单项可以剪切粘贴了;移动端菜单和磁贴滑动切换；
* 180122 可选高性能模式（禁用一些模糊和半透明）
* 180122 优化背景图片渲染效率；优化了取色器的数据交互，自动回传颜色值；
* 180118 手机端时，应用最大化,插件隐藏到底部;修复窗口通信bug；
* 180117 修改了系统设置的响应式;
* 180116 图标样式微调,做了一点点响应式;
* 180115 磁贴的基本样式；IE下，提高不透明度；
* 180112 快速添加网址到新建应用;完善菜单项drawer的图标样式;分组的重命名
* 180111 桌面图标和菜单可以相互复制子项，都可以高级配置了;窗口交互和通信模块完成；新开的窗口稳定浮于上面;
* 180109 部分窗口交互代码;vue.min.js进行了格式化，修复了IE的未知原因的bug;子页使用child.js后可以F5刷新自身；更好的子页刷新动画;app运行脚本添加了用户信任的限制；
* 180108 winSetActive设置了200ms的惰性检测;可视化添加app;应用管理的同步；添加resizable属性；微调窗口样式；添加调色板app；
* 180105 应用管理的前端;
* 180104 移除win的window属性（用不上）;带参数地打开窗口;根据app的启动源，可记录位置和大小;新增窗口是否可resize;layer皮肤;更多动画;beforeOpen..等函数添加了第二个形参win;更好的urlBuilder;winOpend改为监听属性
* 180103 美化了loading界面，添加更多的预加载；
* 180102 为默认壁纸添加了缩略图;管理中心打开时也模糊桌面;小便签工具;优化了过渡动画；支持图片图标；
* 171229 子页刷新时通过产生一个随机token来禁用缓存;减少父页对子页postMessage的自由度（eval改select）,解决跨域页面的安全隐患
* 171228 针对IE修复了Vue一些冲突的代码，修复了一些css，并对不能高斯模糊这一点表强烈谴责；
* 171225 清空消息加了动画;实时保存到localStorage；修正msg的预览html不解析的bug；简单的读取get的autoSave值来决定存档位置；抽屉的z-index设置为99999，解决了动态计算带来的卡顿；优化了一些css
* 171225 圣诞节！初步完成数据管理，已实现导入导出json文件，保存、读取localStorage；
* 171222 完成序列化和导入导出功能，数据格式统一为json；删除了一些冗余代码；重构初始化代码，添加函数onLoad和onReady对应资源文件加载完毕和实例化完毕后触发。
* 171220 添加YL.ready()函数，在init前调用；自启动的实现和管理；设置页的图标也使用组件了，需要注意模板统一；
* 171214 多级菜单组件完成；添加全屏的API；
* 171213 壁纸可简单添加/删除；磁贴列数可自定义（但是保存并刷新生效）；图标组件化；菜单组件化；
* 171211 小游戏“太空防御者”的编写
* 171208 引入element-ui，完善主题色设置；单例会激活已打开的窗口；完成壁纸设置功能；
* 171207 优化子窗口css，开始菜单全屏打开并隐藏普通窗口
* 171206 开始菜单全屏化；磁贴自适应尺寸；背景模糊效果；菜单关闭逻辑优化
* 171205 可以将插件置底，作为背景，不可交互；统一了窗体右键菜单；优化窗体样式
* 171204 任务栏右键置顶或置底
* 171123 父子页可以通过postMessage的API通信（yl.app.js）;添加窗体地址栏;开始菜单右键窗体添加“窗体置中”；子窗口点击置顶
* 171120 为菜单、磁贴、消息中心添加了滚动条插件;任务栏可置顶；标题文字省略号；loading界面
* 171117 可以从应用管理往桌面加图标了;为了统一，固定了菜单宽度，暂时禁用了横向缩放；图标右键添加磁贴；
* 171116 插件可以记住位置了；抽屉图标也有对应的右键菜单；双击窗口标题最大化；引用组件vue-grid-layout用于高级磁贴；优化了组件加载（尤其是layer的特殊加载方式）
* 171020 窗口实例不再依赖app引用，可以临时创建一个窗体；app管理雏形
* 171023 右下角消息提示改为框式

### 踩坑记录
* IE11 需要受信任才能使用localstorage?安全设置的问题
* IE11 blur的方法？答：只能对图片模糊，鸡肋
* IE11 z-index不按常理，在父级加入样式z-index:0
* IE11 鼠标拖动触发的事件结构不太一样(vue)
* IE11 不支持filter:blur (脑残？？)
* IE11 不支持link prefetch 的onload回调
* IE11 iframe的src有hash（锚点）的情况下，document.activeElement居然是错误（喵喵喵？），任何试图读取它的代码都会导致致命错误；解决方案：提前element.focus()
* IE11 vue.min.js莫名其妙的报错，格式化后修复；推测为js编译器辣鸡
* FUCK IE
* Chrome字体必须是100%（默认）
* url尽量使用全路径（带协议,带index.html）
* 图标改为数组不是个好主意，需要唯一标识方便增删操作
* 谷歌浏览器最新版样式比起旧版有细微差别，另外在磁贴中，height 100% 的 iframe发生溢出，父容器高度设为99%解决，原因未知
* 遍历数组条件删除元素可以使用倒序遍历来避免splice出错的问题