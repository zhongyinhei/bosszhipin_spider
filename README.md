# BOSS直聘网站爬虫脚本

## 环境要求
- Python 3.7.0
- request
- BeautifulSoup

## 爬虫脚本1 —— company_salary.py
### 主要功能
1. 针对16种常见热门语言和27个中国较大型互联网企业的岗位需求分别进行爬取。

2. 针对每一家公司和每一种语言，最终提取以下信息:
>   - 平均薪资水平
>   - 最高薪资
>   - 最高薪资岗位
>   - 最低薪资
>   - 最低薪资岗位

3. 除上述信息外，仍存在隐式信息，包括岗位地点，每一种岗位具体名称和薪资等，在每一轮爬取过程中，如下表所示：
> - 岗位名称 spider.job
> - 岗位具体薪资 spider.money
> - 岗位地点 spider.place

4. 爬取过程中进行了一定的数据清洗，处理掉了大部分的非技术岗位需求。

### 运行方法
`python company_salary.py`

## 爬虫脚本2 —— language_post.py
### 主要功能
1. 针对16种热门语言BOSS直聘上的热门高质量岗位进行爬取。

2. 针对每一种语言，提取6个名称不同的岗位。 针对每一条记录，内容信息包括：
> - 岗位名称
> - 薪资水平

### 运行方法
`python language_post.py`

## 备注
### 支持爬取的语言(排名不分先后)：
C++, Java, Python, R语言, Go, Matlab, Scala, VB.NET, SQL, Objective-C, C, Ruby, PHP, 汇编, C%23, Javascript

### 支持爬取的公司(排名不分先后):
字节跳动, 阿里巴巴, 华为, 腾讯, 金山, 百度 ,京东, 滴滴出行, 小米, 360, 美团, 网易, 拼多多, 携程, 新浪, 苏宁易购, 快手, 唯品会, 陆金所, 科大讯飞' 58, 汽车之家, 爱奇艺, 链家网, 哔哩哔哩, 斗鱼, 迅雷
