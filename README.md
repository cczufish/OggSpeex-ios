OggSpeex-ios
============
iOS和android speex语音压缩以及ogg封装

什么是ogg和speex：

Ogg全称应该是OGGVobis(oggVorbis)是一种新的音频压缩格式，类似于MP3等的音乐格式。Ogg是完全免费、开放和没有专利限制的。OggVorbis文件的扩展名是".ogg"。Ogg文件格式可以不断地进行大小和音质的改良，而不影响旧有的编码器或播放器。      详细介绍：http://baike.baidu.com/link?url=U1k5teU4TcPQS0pF5yto6PgDrTgXo5xLewTDNOJiKSeJqH3mSw_Kdgn30z8K7aSd

speex：
Speex是一套专门用于压缩声音的库,由于其专门针对声音,所以压缩声音的性能非常高.Speex由于其压缩性能,及0.80版后的跨平台的性能,所以在网络声音的传输中有很大的价值.但是需要注意的是speex只能对声音进行压缩,不支持音乐的压缩,如果你需要音乐的压缩你或许需要用vorbis库.支持包括Linux、BSD、MacOS 以及 Symbian 系统。http://www.baidu.com/s?tn=baiduhome_pg&ie=utf-8&bs=ogg&f=8&rsv_bp=1&wd=speex&rsv_sug3=6&rsv_sug=0&rsv_sug1=2&rsv_sug4=1226&inputT=1573

首先上demo：别人写的  http://code4app.com/ios/speex语音压缩以及ogg封装/52139e0a6803fa4503000000    使用 speex 格式对录制的声音进行语音压缩，并且进行ogg封装，实现了 ios 和 android 的语音编解码互通。代码包包括iOS Demo 和 Android demo。

相关speed技术介绍：  http://blog.csdn.net/zsjum/article/details/7494548   http://blog.csdn.net/zsjum/article/category/929394

音频编解码之speex－speex编译静态库for iOS        http://blog.sina.com.cn/s/blog_674f4fc6010112a4.html

开源语音格式speex教程  http://www.cocoachina.com/bbs/read.php?tid=114755

其实我理解的逻辑就是：speex.encode()成byte[]，然后通过网络发出去，接收到了之后再speex.decode()完就可以播放了。
