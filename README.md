#爬取豆瓣标签下的书籍。

1.爬虫分为3个模块：日志模块，资源模块，爬虫模块。
    a.日至模块是爬虫的日志系统。
    b.资源模块存放的是连接mysql的配置，User-Agent和代理ip。
    c.爬虫模块，是爬取需要的数据，保存到mysql和Excel表格中。

2.反爬虫的措施:
    a.使用随机User-Agent，模拟浏览器请求。
    b.使用随机代理ip访问。
    c.为防止访问频繁，通过4个线程爬取，每个线程延时1-3秒爬取。爬取的数据通过两个线程进行保存。

3.工作环境
    架构：X86-64
    系统：Fedora 26
