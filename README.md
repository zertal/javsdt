# jav-standard-tool 简称javsdt
# 作者为生活所迫，已经跑路...
简介：收集jav元数据，并规范本地文件（夹）的格式，收集女优头像，为emby、kodi、jellyfin、极影派等影片管理软件铺路。  

  
1、下载及群链接：  
    目前2020年3月18日更新的1.0.6版本  使用环境win7/win10 64位  
    [前往下载exe](https://github.com/junerain123/javsdt/releases/tag/V1.0.6)或者[从蓝奏云下载](https://www.lanzous.com/iaed6ad)  
  
    [前往下载演员头像](https://github.com/junerain123/javsdt/releases/tag/女优头像)   
  
    [电报群](https://t.me/javsdtool)  
    [企鹅群](https://jq.qq.com/?_wv=1027&k=5CbWOpV)（需要付费1人民币入群）  
  
2、其他开发者：  
    python3.7 使用pyinstaller打包成发行版exe  
   pip install requests  
   pip install Pillow  
   pip install baidu-aip  
   pip install pysocks  
   pip install cfscrape  
    几个jav的py都是独立执行的，加了很多很多注释，希望能理解其中踩过的坑。  
  
3、工作流程：  
    （1）用户选择文件夹，遍历路径下的所有文件。  
    （2）文件是jav，取车牌号，到javXXX网站搜索影片找到对应网页。  
    （3）获取网页源码找出“标题”“导演”“发行日期”等信息和DVD封面url。  
    （4）重命名影片文件。  
    （5）重命名文件夹或建立独立文件夹。  
    （6）保存信息写入nfo。   
    （7）下载封面url作fanart.jpg，裁剪右半边作poster.jpg。   
    （8）移动文件夹，完成归类。  
  
4、目标效果：  
![image](https://github.com/junerain123/Collect-Info-and-Fanart-for-JAV-/blob/master/images/1_files_origin.png)  
![image](https://github.com/junerain123/Collect-Info-and-Fanart-for-JAV-/blob/master/images/2.png)  
![image](https://github.com/junerain123/Collect-Info-and-Fanart-for-JAV-/blob/master/images/3.jpg)  
  
5、ini中的用户设置：  
![image](https://github.com/junerain123/Collect-Info-and-Fanart-for-JAV-/blob/master/images/4.PNG)  
  
6、其他说明：  
（1）不需要赞助；  
（2）允许对软件进行任何形式的转载；  
（3）代码及软件使用“MIT许可证”，他人可以修改代码、发布分支，允许闭源、商业化，但造成后果与本作者无关。  
