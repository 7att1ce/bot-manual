# OSU查询功能

> OSU查询功能的设计之初想要兼容一些目前用的比较多的机器人的命令，比如白菜，猫猫。
>
> 后续可能会更改一些东西，不再保持兼容性。
>
> OSU!API使用文档：[https://osu.ppy.sh/docs/](https://osu.ppy.sh/docs/)

## 绑定OSU账户

`!setid <osu_id>`

osu\_id为osu账户的用户名。

在使用一些其他命令时如果没有指定用户名，则会查询社交账号绑定的OSU账户。

## 设定默认的游戏模式

`!setmode <mode>`

mode为游戏模式的数字，具体情况如下

* 0: std模式，戳泡泡模式
* 1: taiko模式，太鼓模式
* 2: fruits模式，接水果模式
* 3: mania模式，下落式

绑定OSU账户后可以指定查询是默认的游戏模式，如果没有设置则默认为std模式。

## 查询账户个人资料

`!info[:<mode>]`

`!info <osu_id>[:<mode>]`

osu\_id，mode含义同上

mode缺省时默认为std模式或者绑定账户的默认模式

查询结果以图片的形式返回

## 查询最近成绩

`!pr[:<mode>]`

`!pr <osu_id>[:<mode>]`

osu\_id，mode含义同上

mode缺省时默认为std模式或者绑定账户的默认模式

查询结果以图片的形式返回

## 查询最近成绩（包括未pass成绩）

`!recent[:<mode>]`

`!recent <osu_id>[:<mode>]`

osu\_id，mode含义同上

mode缺省时默认为std模式或者绑定账户的默认模式

查询结果以图片的形式返回

## 查询指定bid的成绩

`!score <bid>`

bid为beatmap id

只有Rank和Loved谱面支持此功能

查询结果以图片的形式返回

## 查询bp

`!bp[[#<num>]:<mode>]`

`!bp <osu_id>[[#<num>]:<mode>]`

osu\_id，mode含义同上

num含义为bp从大到小的排名，缺省为1，即bp榜最高pp的成绩

查询结果以图片的形式返回

