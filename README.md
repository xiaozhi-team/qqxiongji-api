# QQ 凶吉 API

QQ 凶吉

提交 QQ，返回 QQ 凶吉，主人性格

最新源码在`Releases`

欢迎各位下载

<a href="https://gitee.com/XiaoZhi_Studio/qqxiongji-api/stargazers"><img src="https://gitee.com/XiaoZhi_Studio/qqxiongji-api/badge/star.svg?theme=gvp"></a>

返回示例（json）：

```
    {
        "code": "1",
        "text": "获取成功",
        "data": {
            "uin": "10001",
            "evaluate": "云开见月，虽有劳碌，光明坦途，指日可望 ",
            "luck": "吉",
            "master": "[热情/善变梦想家型]，其具体表现为：对人热情无遮掩，时常梦想可以谈一场戏剧性恋爱，亲身体会个中悲欢离合的动人经历，是个大梦想家。但对于感情却易变卦。"
        }
    }
```

返回示例（text）：

```
QQ号：10001

号码凶吉：云开见月，虽有劳碌，光明坦途，指日可望 

是为：吉

主人性格：[热情/善变梦想家型]，其具体表现为：对人热情无遮掩，时常梦想可以谈一场戏剧性恋爱，亲身体会个中悲欢离合的动人经历，是个大梦想家。但对于感情却易变卦。
```

提交信息：

| 名称 | 必填 | 类型 | 说明 |
| ------- | ------- | ------- | ------- |
|qq|是|string|QQ号|
|type|否|string|留空为JSON，type可为json或text|

返回参数：

| 名称 | 类型 | 说明 |
| ------- | ------- | ------- |
|code|string|状态码
|text|string|状态，获取成功为请求成功>
|uin|string|QQ号
|evaluate|string|号码凶吉
|luck|string|凶/吉
|master|string|主人性格|

请求示例：

text:http://xxx.com/xiongji.php?qq=10001&type=text

json:http://xxx.com/xiongji.php?qq=10001&type=json

> API：[小职 API](http://api.83883.top/)

> 接口调用：[qqxiongji.bmcx.com](https://qqxiongji.bmcx.com/)
