![plugins-for-nonebot2](https://socialify.git.ci/beiyuouo/plugins-for-nonebot2/image?font=Source%20Code%20Pro&forks=1&issues=1&language=1&logo=https%3A%2F%2Favatars0.githubusercontent.com%2Fu%2F44976445%3Fs%3D460%26u%3D182d335f502ab38522bde613717bd77aa1f6f766%26v%3D4&owner=1&pattern=Circuit%20Board&pulls=1&stargazers=1&theme=Light)

<!-- MarkdownTOC -->

- [Plugins for nonebot2](#plugins-for-nonebot2)
- [Changelog](#changelog)
    - [20210122 v0.1.0](#20210122-v010)
    - [20210116 v0.0.4](#20210116-v004)
    - [20210114 v0.0.3](#20210114-v003)
    - [20210114 v0.0.2](#20210114-v002)
    - [20210113 v0.0.1](#20210113-v001)
- [TODO](#todo)
- [插件说明](#%E6%8F%92%E4%BB%B6%E8%AF%B4%E6%98%8E)
    - [menu](#menu)
    - [base](#base)
    - [rp](#rp)
    - [ssr/v2ray](#ssrv2ray)
    - [v2raycs](#v2raycs)
    - [twqd](#twqd)
    - [ai](#ai)
    - [ai_100000000](#ai_100000000)
    - [bullshit](#bullshit)
    - [zhihu](#zhihu)
    - [twqh](#twqh)
    - [auto_agree](#auto_agree)
    - [setu](#setu)
    - [helpme](#helpme)
    - [souti](#souti)
    - [tiangou](#tiangou)
    - [weather](#weather)
    - [mrwh](#mrwh)
    - [yiqing](#yiqing)
    - [hhsh](#hhsh)

<!-- /MarkdownTOC -->

## Plugins for nonebot2

自用插件（确信）

测试机器人QQ851722457

有啥好的插件想法/独家定制请发issue 0.0

## Changelog

### 20210122 v0.1.0
- 代码重构，更新配置方式，更易于移植和配置

### 20210116 v0.0.4
- 添加`hhsh`和`menu`功能

### 20210114 v0.0.3
- 仓库重命名为bbot

### 20210114 v0.0.2
- 添加`menu,mrwh`和`setu`功能

### 20210113 v0.0.1
- 基础框架和功能

## TODO

- [x] 重构
- [x] 配置文件，易部署修改
- [x] 异常处理
- [ ] 命令的模糊匹配

## 插件说明

### menu

说明：插件汇总，菜单

命令：`{ menu | 菜单 }`

### base
说明：基础命令，由于目前食用的nonebot2版本builtin插件有问题，因此做了简单的重写

命令：`{ say | echo } { text }`

### rp
说明：测试用插件，`(1,100)` 随机数

命令：今日人品

### ssr/v2ray
说明：获取一条ssr/v2ray链接，API配合<a href="https://github.com/QIN2DIM/V2RayCloudSpider">V2RayCloudSpider</a>食用

命令：`{ ssr | v2ray }`

食用指北：修改`.env.dev`内配置ssr/v2ray/v2raycs的api接口

### v2raycs
说明：获取ssr/v2ray余量信息，API配合<a href="https://github.com/QIN2DIM/V2RayCloudSpider">V2RayCloudSpider</a>食用

命令：`v2raycs`

### twqd
说明：HainanUniversity体温签到接口，详见<a href="https://github.com/beiyuouo/hnu-temp-report-bot">hnu-temp-report-bot</a>

命令：
```
twqd { 学号 }
twqdall
adduser { 学号 } { 密码 } { 邮箱 }
add { 学号 } # 以发送人QQ为键值
add { qq } { 学号 }
query { qq | 学号 } {}
```

### ai
说明：百度UNIX2，图灵机器人接口

命令：`""`，正常对话即可

食用指北：修改`.env.dev`内的BAIDU_API_KEY等

### ai_100000000
说明：价值一个亿的AI核心代码，dddd

命令：`ai {}`


### bullshit
说明：狗屁不通生成器

命令：`{ bullshit | 狗屁不通 | 狗屁不通生成器 } { theme }`

### zhihu
说明：知乎日报

命令：`{ zhihu | 知乎 | 知乎日报 }`

### twqh
说明：来一句土味情话

命令：`{ twqh | 土味情话 | 情话 | 土味 | 来句土味 | 来句情话 | 来句土味情话 | 你爱我吗 | 爱我吗 }`

### auto_agree
说明：自动同意好友申请和加群邀请

### setu

说明：给俺来张瑟图！

命令：`{ setu | 瑟图 | 色图 | 来张瑟图 | 来张色图 }`

### helpme
On Developing...

说明：帮我

命令：
```
帮我骂人 @someone
```

食用指北：添加`脏话样本.txt`

### souti

On Developing

说明：搜题

命令：
```
搜题 { 题目 }
```

食用指北：


### tiangou

On Developing

说明：来舔我

命令：

食用指北：


### weather

On Developing

说明：天气预报

命令：

食用指北：

### mrwh

说明：每日问好，用到的插件<a href="https://github.com/nonebot/plugin-apscheduler">https://github.com/nonebot/plugin-apscheduler</a>

命令：无

食用指北：
修改`.env.dev`文件中
```
MRWH_GROUP = [''] # 需要通知的群列表
MRWH_SPECIAL_USER = [''] # 需要特殊提醒的群成员
TIANQI_KEY = '' #Tianqi API Key
```


### yiqing

On Developing

说明：疫情查询

### hhsh

说明：能不能好好说话？

命令：`hhsh { text text }`

