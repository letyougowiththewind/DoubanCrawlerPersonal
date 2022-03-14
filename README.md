# DoubanCrawlerPersonal
这是一个用于爬取自己标记已看过的豆瓣电影的程序，设计有随机时间的爬虫休息机制。
## 简介

爬取豆瓣“我看过的电影”页面的影视条目信息，包括标题、IMDb ID、打分、标记时间、标签、短评，并制成.csv

## 使用方法

### 方法一

- 直接运行main.exe文件；

### 方法二

- 安装python3环境；
- pip安装requests、beautifulsoup4和lxml这三个第三方库；
- 运行main.py；

## 用法

1. 填写自己的用户id，在地址栏中可以看到；
2. 填写豆瓣用户cookies，在控制台network中找寻；
3. 选择对第几页到第几页进行备份；
4. 输入文件名创建csv文件，挂机等待抓取结束；
5. 打开csv文件，将标记时间那一列的单元格格式改为“yyyy-mm-dd”

## 注意

1. 爬虫速度设置得很慢，建议多次少页。
2. 两种情况将导致缺少IMDb ID，一是条目本身无IMDb编号，二是条目已被404。建议CSV保存完毕后自行进行检查和补上。
3. 如果填写的csv文件名在同目录下存在同名文件，将会对同名文件进行覆盖。
