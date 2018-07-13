# compiled_ijkplayer4android
基于ijkplayer编译，以支持ijkplayer默认不支持的avi，mpg等视频格式。本项目可以下载后自行编译，也可以只下载编译好的so直接使用。  
   
编译后的so路径:`android/ijkplayer/ijkplayer-abi_name/src/main/libs/abi_name`    
  
如需要armabi-v7a的so，其路径为`android/ijkplayer/ijkplayer-armv7a/src/main/libs/armabi-v7a`,下载该文件，拷贝到项目的对应目录中即可，其他abi依次类推。  


ijkplayer的默认用法如下：  
```
compile 'tv.danmaku.ijk.media:ijkplayer-java:ijk_version'
compile 'tv.danmaku.ijk.media:ijkplayer-armv7a:ijk_version'
// other abis
// compile 'tv.danmaku.ijk.media:ijkplayer-armv5:ijk_version'
// compile 'tv.danmaku.ijk.media:ijkplayer-arm64:ijk_version'
// compile 'tv.danmaku.ijk.media:ijkplayer-x86:ijk_version'
// compile 'tv.danmaku.ijk.media:ijkplayer-x86_64:ijk_version'
```
因为这里使用自己变得so，所以远程so依赖可以删除，java api继续使用即可。  
```
compile 'tv.danmaku.ijk.media:ijkplayer-java:ijk_version'
// 删除远程so依赖
// compile 'tv.danmaku.ijk.media:ijkplayer-armv7a:ijk_version'
// other abis
// compile 'tv.danmaku.ijk.media:ijkplayer-armv5:ijk_version'
// compile 'tv.danmaku.ijk.media:ijkplayer-arm64:ijk_version'
// compile 'tv.danmaku.ijk.media:ijkplayer-x86:ijk_version'
// compile 'tv.danmaku.ijk.media:ijkplayer-x86_64:ijk_version'
```  
  
# 博文地址  
[《Android开发小记：编译ijkplayer以支持更多视频格式》](http://blog.csdn.net/Xiong_IT/article/details/78066995)

# 更新日志
20180713  
更新ijkplayer为v0.8.8  

20170922  
基于ijkplayer v.8.3

