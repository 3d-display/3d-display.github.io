# 世锟裸眼3D-DISPLAY

## [点击下载](https://raw.githubusercontent.com/3d-display/3d-display.github.io/master/%E8%A3%B8%E7%9C%BC3D-DISPLAY-RC9.apk)

### 根据google-exoplayer定制的裸眼3D播放器  

- 支持4K硬解码   
- 支持无缝播放   
- 支持开机自动播放
    - 播放器默认为4K硬解码开机自动无缝播放，支持最大分辨率3840x2160。
- 支持ud格式视频
    - 视频文件的文件名中，需要包含字母ud/UD，视频将自动识别为上下格式的视频。
- 支持2dz格式视频
    - 视频文件的文件名中，需要包含字母2dz/2DZ，视频将自动识别为2d+z格式的视频。
- 支持lrv格式视频
    - 视频文件的文件名中，需要包含字母lrv/LRV，视频将自动识别为左右格式的视频。
- 支持9grid格式视频
    - 视频文件的文件名中，需要包含字母9grid/9GRID，视频将自动识别为九宫格格式的视频。
- 3288与3399兼容支持
    - 3288支持上述所有格式，3399支持除UD之外的所有格式。
- 插入U盘自动拷贝视频
    - 操作步骤：① 在U盘根目录创建名为“_video”的文件夹 ②在创建好的“_video”文件夹中新建txt文件，文件名称可以是“1.txt”或“2.txt”或“3.txt”，分别对应三种不同的拷贝模式。③ 将U盘插入机器的USB接口中，即可开始自动拷贝视频。
    - 三种模式：     
          * 模式1：U盘 ——> 机器   
          * 模式2：机器 ——> U盘   
          * 模式3：U盘 ——> 机器（覆盖以前的内容）  
- 自动读取加密的配置参数文件
    - 播放器的配置参数文件保存在广告机中，位置为 ———— /MouHe/conf/mouhe.pwd
    - 注意请不要自行删除该配置文件，否则播放器无法正常运行！！！
- 自动播放指定文件夹下的视频  
    - 播放的视频文件保存在广告机中，位置为：———— /MouHe/
- 支持3288景深调节（2DZ）
    - 广告机正在播放视频时，可以点击鼠标右键，返回到2DZ格式视频的景深调节界面，点击景深调节，设置景深并保存即可。
- 支持的视频格式：MP4、M4A、FMP4、WebM、MKV、MP3、Ogg、WAV、MPEG-TS、MPEG-PS、FLV和ADTS (AAC)
    - 详细说明：
    - By default Player uses Android’s platform decoders. Hence the supported sample formats depend on the underlying platform rather than on ExoPlayer. Sample formats supported by Android devices are documented here. Note that individual devices may support additional formats beyond those listed.
    - 默认格式说明：
    - https://google.github.io/ExoPlayer/supported-formats.html （需翻墙）
    - https://developer.android.google.cn/guide/topics/media/media-formats#core (国内地址)
- 常见问题：
    1. 视频无3D效果
        - 解决办法：  
        ① 请检查文件名是否正确  ② 请检查配置文件的参数是否为正确（参数不能为空，线数跟倾角不能为零） ③ 如果是3288板型，请检测IIC通信的线路是否正常
    2. 播放器开机不自动启动 
        - 原因：应用无法接收到开机广播。
        - 解决办法：① 应用程序安装后重来没有启动过，这种情况下应用程序接收不到任何广播。① 应用安装到了sd卡内，安装在sd卡内的应用是收不到开机广播的。③ 系统开启了Fast Boot模式，这种模式下系统启动并不会发送开机广播。
    3. 插入U盘不自动拷贝视频
        - 解决办法：① 请检查“_video”文件夹名称是否正确 ② 请检查“_video”文件夹中，是否存在1.txt或2.txt或3.txt文件。 
