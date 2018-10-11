# 解决Mac上用spotlight搜索输入几个字母后闪退问题
>源自：[开源中国](https://my.oschina.net/u/1037903/blog/2221932)

> 问题描述：使用spotlight进行搜索时，只要输入字母超过一定个数(在我的Mac上是5个左右)，spotlight就闪退了。

谷歌搜索得到大部分解决方案是在系统自带词典的偏好设置里取消外部字典的勾选(如[https://placeless.net/2017/09/28/spotlight-search-crash-on-high-sierra.html](https://placeless.net/2017/09/28/spotlight-search-crash-on-high-sierra.html))。
但实际操作发现这个并不能解决我Mac上的问题。

:yellow_heart:**解决方法**：  
    按苹果官网上关于这问题的讨论([https://discussions.apple.com/thread/8546951](https://discussions.apple.com/thread/8546951))
可能是近期Safari的升级所致，需要在spotlight的设置里取消书签与历史记录(Bookmarks & History)的勾选，即系统偏好设置-Spotlight-搜索结果-书签与历史记录(Bookmarks & History)取消勾选。

