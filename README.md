# auto_feed_js
PT站一键转载脚本

### 前言

----

不知不觉，这个脚本已经快一年了，期间收获了很多，起初只是极个别人找到我说帮忙写，后来越来越多，然后现在是给了猫站发布组，也给了柠檬发布组。我的初衷肯定是希望公开的，只是有一种担忧需求越来越多，个人会比较吃不消，尤其自己处在挣扎毕业阶段。

### 众人拾柴火焰高

----

知识共享时代，我的PT理念是自己喜欢的资源自己去发布，然后喜欢的人下载，一起保到天荒地老。很欣喜看到PTPP和IYUU这样的工具出来，帮助大家愉快的畅玩PT，自己也欣然共享。

### 更新日志

----


+ 版本 v1.0
  
  > 20200417：新增支持外站PHD和avz作为源站点; (by tomorrow505)
  > 20200420：新增馒头、猫站、春天、听歌、瓷器、我堡发布页面填写匹配 (by tomorrow505)
  > 20200422：新增pthome、hdhome发布页面填写匹配; 修复我堡部分bug (by tomorrow505);新增天空、岛、联盟发布页面匹配 (by hollips)

    
+ 版本 v1.1
  
  > 20200424：新增MTV作为源站点, 新增ptp作为源站点(待测试) (by tomorrow505) ——> 已测试
  > 20200425：新增一键打开常用站点的功能，需要设置common_sites (by tomorrow505)
  > 20200427：修复CMCT新种子页面mediainfo信息异步加载获取不到的bug; 添加ptgen跳转，主要是为了方便外站查询信息 (by tomorrow505)

   
+ 版本 v1.2

  > 20200429：修改获取豆瓣信息的代码，使用promise进行链式简化;从副标题匹配是否包含国语粤语中字等信息并勾选标签 (by tomorrow505)
  > 修复league(柠檬)分类更新导致错误分类的bug; 修复HDT有多个重复发布的资源获取类别错误的bug (by tomorrow505)
  > 20200430：新增支持南洋、葡萄、TLF、杜比发布页填写匹配;完善官种感谢机制,在reg_team_name补充官方小组后缀名即可; 
  > 修复猫站官种转发table到其他站点混乱的bug (by tomorrow505)

  
+ 版本 v1.3

  > 20200501：修复插入节点不在常规位置的bug;修复cmct因为图片元素节点更名获取不到图片的bug (by tomorrow505)
  > 修复HDT部分bug; 修复豆瓣获取button部分bug; 新增：瓷器没有豆瓣信息插入获取豆瓣获取button (by tomorrow505)
  > 支持：萌猫——匹配一部分，因为是二级勾选，然后比较繁琐…… (by tomorrow505)
  > 20200506: 匹配HDT原盘转发到春天。 (by hollips)

+ 版本 v1.4

  > 20200531: 修复TTG官种wiki转出图片未加载的bug; 修复猫站转出带站点转出链接提示的bug. (by tomorrow505)
  > 增加北洋作为源站点的部分修复，支持北洋作为发布站点; 新增UHD作为源站点，费老劲了(by tomorrow505)
  > 20200606: 新增blutopia为源站点 (by tomorrow505)
  > 20200703：新增TCCF为发布站点；修复: 葡萄北洋默认勾选匿名。  (by tomorrow505)
  > 20200713：大致支持印度站点hon3yhd，新增api替换选项。  (by tomorrow505)
  > 20200714：烧包支持，海胆支持，diy标签支持；匿名整合作为用户选项。  (by tomorrow505)

+ 版本 v1.5
  
  > 20200715：支持蝴蝶转发及转出，可惜只能校内用户登录及IPV6用户(带有不确定因素)~; 支持HDFANS转发。 (by tomorrow505)
  > 20200722：加入IPT进入豪华套餐。  (by tomorrow505)
  > 20200723：加入xthor作为外网源站点，感谢贝壳大佬发邀。 (by tomorrow505)
  > 20200724：支持hdroute..感谢假装大佬测试。佛曰：不可说; 修复萌猫的部分bug，修复其他站点部分bug。 (by tomorrow505)
  > 20200725：支持Filelist作为源站点，感谢宝大发邀。 (by tomorrow505)

  > 20200729：修复UHD原盘转发命名错误的bug,但是仍旧可能不准确，TL缺少mediainfo基本无解。 (by tomorrow505)
  > 20200804：修复北邮人转出部分bug, 修复hon3yhd小组DRs原盘命名。 (by tomorrow505)
  > 20200811：修复CMCT，对新版适配更加方便。 (by tomorrow505)
  > 20200814：新增支持HDPOST、HDCity，整合代码提取两个函数。修复部分bug. 完善HDFans，完善海胆(by tomorrow505)

  > 20200820；由于imdb转豆瓣解析api失效，暂时没有更好的办法，对外站获取豆瓣信息做了一丢丢修复工作。(by tomorrow505)
  > 20200827：修复ptgen跳转出错问题、修复HDT失效问题。 (by tomorrow505)
  > 20200828：修复PThome分辨率选择增加8K导致的错误，修正类别为动画或者纪录片获取初始为电影的错误; 修复HDHome原盘转载媒介错误的bug。整合精简部分代码。 (by tomorrow505)
  > 20200829：新增支持发布到BHD，截图部分需要自行解决。 (by tomorrow505)
  > 20200903：新增支持HDF作为源站点，但是基本缺少截图;简单修复ptgen跳转获取不到豆瓣信息的问题。 (by tomorrow505)
  > 20200908：新增支持RED和皇后作为源站点，简单适配发布到柠檬及其他站点;简单音乐转载的修复部分bug, 修复皇后有两种版面-老种不规范带来的部分bug。

  

+ 版本 v1.6

  > 20200923：萌猫关站, 不再支持萌猫;支持U2作为源站点转外。
  > 20200926：支持HDB作为源站转发。优化外站电视剧转载非第一季获取豆瓣过程，勾选API进行检索即可获得备选豆瓣链接。
  > 20200927：支持BTN作为源站转发，基本集齐。
  > 20200928：新修复一堆bug，以后大伙使用有bug可以直接给我抛链接和描述，尽量及时修复。
  > 20201001：新增支持兽站、CCF、HDTime、龙之家、52PT、影客、伊甸园、PTMSG、铃音、碟粉、JoyHD、HDZone、Oshen、HDAtmos、PTNIC作为发布站点。
  > 20201002：新增支持发布到HDT，简单适配。修复bug一堆。    

  > 20201019：高清街关站，不再支持。
  > 20201027：新增Bdc为源站点，blutopia为发布站点(需要申请TMDB的api)、AHD。
  > 20201115：修复柠檬，增加UHD作为发布站。

  > 20201119：支持转发到HDSpace，取消支持IPT, 太混乱了。修复其余bug多项，完善PTP原盘命名，支持多个站点下载截图(外站很慢)。
  > 20201129：简单适配KG电影类别。

  > 20201227：修复柠檬域名,修复柠檬查重, 修复CMCT跳转查询,豆瓣页面新增跳转查询。
  > 20210104：支持elite-tracker, 修复cmct转出感谢多次的bug。

  > 20210308：取消对AHD的支持，修改HDPOST新架构的支持。
  > 20210312：支持1PTBA、HITPT、PTtime(shmt86)、简单支持iTS(感谢黑白大佬提供帮助)->已经完善。 取消支持影客(关站)。
  > 20210316：重构部分代码，用户变量提前至顶端，可以方便更改自己的配置; 
  > 20200318：修复HDT的图链bug一枚，修复BLU等相似架构搜索问题。


+ 任务：
  
  > 接下来想要做的事：完善各个块的代码逻辑(尤其是发布页形成函数封装)，源页面干掉外站ajax,重构代码ing...
  > 完善mediainfo和截图分离函数，大部分外站都需要分离操作；柠檬动漫和音乐改版之后代码需要重新整理。

### 使用介绍

----

与一般的油猴脚本一样，直接使用即可，部分细节可以参考[我的博客](http://tomorrow505.xyz/PT%E5%8F%91%E5%B8%83%E4%B9%8B%E4%B8%80%E9%94%AE%E8%BD%AC%E8%BD%BD%E8%84%9A%E6%9C%AC%E4%BD%BF%E7%94%A8%E6%8C%87%E5%8D%97/)，介绍了一般的使用方案。另外博客也写了一些与PT相关的编程教程，欢迎大家去逛逛。

### 关于打赏

----

为了这个脚本也花了很多时间，如果你喜欢这个脚本，请捐赠我作为更新维护的动力吧。

|                   Alipay                    |                     WeChat                     |
| :-----------------------------------------: | :--------------------------------------------: |
| ![](http://tomorrow505.xyz/img/ali_pay.png) | ![](http://tomorrow505.xyz/img/wechat.png) |

 

