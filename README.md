# CheckIn_BaiduTieba  
百度贴吧签到  
云签到/青龙平台/py  


https://github.com/trw131/TieBaCheckIn  
在前人研究总结脚本基础上，进行了修改：  
1.添加了pushplus的推送  
2.推送内容添加了具体的各个贴吧签到是否成功的内容  
cookie可用时长暂时未知  

前人思路总结：  
根据bduss查找common下的tbs  
根据tbs获取个人关注贴吧列表  
根据个人贴吧列表获取每个贴吧的tbs  
根据签到API进行签到  

使用说明：  
1.获取签到时的cookie，填入py文件中  
    google/edge等浏览器，打开相应贴吧，在该页面，右键-检查-网络，然后点击签到按钮，在其中add请求的标头中，复制cookie内容至py文件  
2.获取bduss，填入py文件中  
    在获取cookie的同页面下，右键-检查-应用，找到BDUSS内容，复制至py文件  
3.server酱/pushplus设置，填写py文件中  
    根据个人使用不同填写key或token即可，具体参考各自网站解释  
4.青龙平台设置  
    脚本管理-上传脚本，定时任务-创建任务-设置脚本位置、定时时间，如"task BaiduTieba.py"、"0 0 8 * * *"，确定即可。  
