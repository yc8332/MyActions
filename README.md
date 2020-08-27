# MyActions
自己用来签到的东东,不支持售后

更新时间:2020-8-27 18:34:10

##
目前已支持[@NobyDa](https://github.com/NobyDa) 以及[@lxk0301](https://github.com/lxk0301) 中京东签到的内容,优点是支持无限数量的京东cookie

## 使用教程

1. 直接fork走
2. 再在`Settings`-`Secrets`里面添加`JD_COOKIE`
3. 多条cookie用`&`隔开，支持无数条cookie

上面三步搞定后就不用管了

刚fork完可能在Actions中看不到对应的workflow

目前已配置好自动执行时间，到了指定时间会执行，并且看到workflow



### Cookie获取和配置

> 具体如何取cookie如何配置,可参考 https://github.com/lxk0301/scripts/issues/8#issuecomment-675837338

```

针对京东cookie我们只需要
pt_key=****;
和
pt_pin=***;
的部分

我有两个京东账号,则我JD_COOKIE里面要填写的内容为
pt_key=****;pt_pin=***;&pt_key=****;pt_pin=***;
```

### Cookie失效通知

目前已接入[@lxk0301](https://github.com/lxk0301)大佬写好的失效通知

可自行接入[server酱的微信通知](http://sc.ftqq.com/3.version)服务

server酱的推送通知服务, 是可选项, 如果需要 自行申请SCKEY,再填入Secrets里面(Name选项输入 `PUSH_KEY` ,Value选项输入申请的 SCKEY)

### fork后如何同步代码

参考

http://www.ibloger.net/article/3361.html

