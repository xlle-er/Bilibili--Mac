<p align="center">
<img height="256" src="https://github.com/xlle-er/Bilibili--Mac/blob/main/src/icon1024.png?raw=true" />
</p>

<h1 align="center">Bilibili</h1>

<p align="center">自制版<b>Mac端</b> Bilibili客户端</p>

<p align=center>
<a href="https://space.bilibili.com/119860884">B站主页</a> ·
<a href="https://github.com/xlle-er/Bilibili--Mac/tags">Releases</a>
</p>

---

## 功能

* 支持视频播放、查找  
* 支持动态查看、排行榜查看
………………  

---

## 制作
    > 哔哩哔哩官方在五月十日推出了Windows版本官方客户端
    > + 该客户端使用electron框架进行制作
    > + 由于此框架支持Windows、Linux、macOS快速移植
    > 于是有了这一自制客户端  
    
![electron](https://github.com/xlle-er/Bilibili--Mac/blob/main/src/electron.png?raw=true "electron官网对此产品描述")
    
### 方法
    
    1. 下载[electron][1]客户端  
    2. 下载[Bilibili][2]官方Windows客户端  
    3. 解压<kbd>.exe</kbd>文件  
    4. 在<kbd>$PLUGINSDIR</kbd>文件夹中找到<kbd>app-64.7z</kbd>压缩文件并解压  
    5. 找到<kbd>~/bili_win-install/$PLUGINSDIR/app-64/resources/</kbd>目录  
    6. 复制<kbd>app.asar</kbd>文件  
![app.asar文件](https://github.com/xlle-er/Bilibili--Mac/blob/main/src/file.png?raw=true "app.asar文件位置")
    7. 解压<kbd>electron.zip</kbd>文件  
    8. 右键<kbd>Electron.app</kbd>,显示包内容  
![显示包内容](https://github.com/xlle-er/Bilibili--Mac/blob/main/src/显示包.png?raw=true "显示包内容")
    9. 将<kbd>app.asar</kbd>文件拷贝到<kbd>～/Electron.app/Contents/Resources</kbd>文件夹中     
    10. 使用Xcode或VScode等代码编辑软件打开<kbd>~/Electron.app/Contents/Info.plist</kbd>文件  
        * 更改内容如下（Xcode为例）：
![更改前](https://github.com/xlle-er/Bilibili--Mac/blob/main/src/更改前.png?raw=true "更改前")
![更改后](https://github.com/xlle-er/Bilibili--Mac/blob/main/src/更改后.png?raw=true "更改后")
    11. 将<kbd>～/Electron.app/Contents/MacOS/Electron</kbd>文件名称改为Bilibili  
    12. 将图标文件
