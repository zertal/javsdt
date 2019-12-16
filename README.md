# JAV-Scraper-and-Rename-local-files
收集jav元数据，并规范本地文件（夹）的格式，为emby、kodi、jellyfin收集女优头像。  
python3.7  使用pyinstaller打包成exe。  
如果要运行py文件，PIL即pillow不要用新版，新版仅支持“png”，我是“pip install pillow==6.0.0”  
百度人体分析的“from aip import AipBodyAnalysis”，aip是“pip install baidu-aip”  
另外需要mac、linux系统下的同志帮忙发布各系统的发行版，要改代码，windows的路径是反斜杠“\”。  

[从release下载windows下的exe](https://github-production-release-asset-2e65be.s3.amazonaws.com/199952692/ea761380-1f46-11ea-8c45-ef75289d2b1b?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20191215%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20191215T062830Z&X-Amz-Expires=300&X-Amz-Signature=e9c11f0054b09c89dbdf3db490d5ed60314a3f26a101aa9a437d9cc8c6dbdc09&X-Amz-SignedHeaders=host&actor_id=44168897&response-content-disposition=attachment%3B%20filename%3DV1.0.0.JAVSDT.zip&response-content-type=application%2Foctet-stream)
  或者[从蓝奏云下载](https://www.lanzous.com/i813bkd)  

[从release下载linux发行版](https://github-production-release-asset-2e65be.s3.amazonaws.com/199952692/0096d900-2006-11ea-957b-03eba64f27c5?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20191216%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20191216T053419Z&X-Amz-Expires=300&X-Amz-Signature=d0d15e740fdcfc778f0446a6d812590028cd38063e151d177161cf540965fd07&X-Amz-SignedHeaders=host&actor_id=44168897&response-content-disposition=attachment%3B%20filename%3D1_5165991216294133825.xz&response-content-type=application%2Foctet-stream)电报群里的人帮忙修改打包的，通过他个人测试，具体情况未知。

[从release下载emby和kodi女优头像](https://github-production-release-asset-2e65be.s3.amazonaws.com/199952692/40b54680-12f9-11ea-94e9-4e37ce4bec6e?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20191203%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20191203T172215Z&X-Amz-Expires=300&X-Amz-Signature=5ecbd9367a7a1135692406957163464a7cfcc9bbd563151bcdc686cceed71aad&X-Amz-SignedHeaders=host&actor_id=44168897&response-content-disposition=attachment%3B%20filename%3Dactors.zip&response-content-type=application%2Foctet-stream)  
  [从release下载jellyfin女优头像](https://github-production-release-asset-2e65be.s3.amazonaws.com/199952692/abfe6180-15f4-11ea-9c0b-cf86d9dc383b?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20191203%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20191203T100311Z&X-Amz-Expires=300&X-Amz-Signature=f13c8e4bd8942884aefe015f369938186147544dfae227fdb07744c64754b655&X-Amz-SignedHeaders=host&actor_id=44168897&response-content-disposition=attachment%3B%20filename%3DPeople.zip&response-content-type=application%2Foctet-stream)  
如果链接失效，请进入[“release”](https://github.com/junerain123/JAV-Scraper-and-Rename-local-files/releases)下载。  

[电报群](https://t.me/javsdtool)  
<a target="_blank" href="//shang.qq.com/wpa/qunwpa?idkey=79a735ccf11ed7f15481ae02f6a58f16315b8b424149455b4dc65868362f4b30">企鹅群</a>  



工作流程：  
1、用户选择文件夹，遍历路径下的所有文件。  
2、文件是jav，取车牌号，到javXXX网站搜索影片找到对应网页。  
3、获取网页源码找出“标题”“导演”“发行日期”等信息和DVD封面url。  
4、重命名影片文件。  
5、重命名文件夹或建立独立文件夹。  
6、保存信息写入nfo。   
7、下载封面url作fanart.jpg，裁剪右半边作poster.jpg。   
8、移动文件夹，完成归类。  

目标效果：  
![image](https://github.com/junerain123/Collect-Info-and-Fanart-for-JAV-/blob/master/images/1.png)  
![image](https://github.com/junerain123/Collect-Info-and-Fanart-for-JAV-/blob/master/images/2.png)  
![image](https://github.com/junerain123/Collect-Info-and-Fanart-for-JAV-/blob/master/images/3.jpg)  

以下为ini中的用户设置：  
  
![image](https://github.com/junerain123/Collect-Info-and-Fanart-for-JAV-/blob/master/images/4.PNG)  
