#这是一款小巧而又强大的分页插件
##插件说明
* 不依赖于jq及其他插件，简单易用，易于拓展维护~
* demo为基于apache服务器实现（主要为异步获取数据）
* 插件样式兼容至IE8及各大主流浏览器

##插件使用
1.初始化<br>
`var pages = new Page(opt)`
> 参数说明
  * pageCon(check):页码存放容器 ——必填参数
  * fbtn(check):首页尾页按钮放置位置 ——out/in   默认out(再外面时显示为自定义首页尾页，在里面时，必须显示为页码)
  * hideNum(check):当页数大于等于多少页时，开始产生省略点 ——默认9
  * prevText:上一页按钮显示的文字 ——默认"<"
  * nextText:下一页按钮显示的文字 ——默认">"
  * firstText:首页按钮显示的文字 ——默认"首页"
  * lastText:尾页按钮显示的文字 ——默认"尾页"
  * selectHandle(check):每次点击选取页码时触发 ——该函数，自动将当前页码值注入函数，接收即可
  * *everyPageNum:每页显示条数 ——默认10
  * *dataCount:数据总条数 ——必填参数
  * 带*号的选项为目前并不确定是否需要支持的功能，需结合api返回数据形式再做决定
  
2.更新页码<br>
`pages.update(pageCount)`
> 参数说明
  *pageCount(check):总页数 ——必填参数
  
3.其他
> 完善备注
  * 参数检测
  * 错误处理
  * 兼容性处理
  * 添加重置page对象方法
