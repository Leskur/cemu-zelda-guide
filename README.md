# 使用 Cemu 游玩《塞尔达传说 旷野之息》
### 为什么创建这个项目？

- 因为我相信您也想在电脑上玩《塞尔达传说：旷野之息》

- 因为网上虽然有很多整合包，但是没有网盘会员下载速度是硬伤

- 因为我希望能学会怎么单独安装某个游戏

于是我尝试了很多方法，找到了一种比较好的方式分享给大家。

### 1. 安装 Cemu - Wii U 模拟器

[Cemu ](https://github.com/cemu-project/Cemu) 是一颗 Wii U 模拟器，能够运行大多数Wii U游戏。

#### 1.1 安装

​	你可以从 [Cemu Release](https://github.com/cemu-project/Cemu/releases) 下载最新的应用程序包并解压到合适的位置，比如 `D:\Games\Cemu`。

​	启动 Cemu 后看会到初始化弹窗，建议直接关闭，先切换成中文之后再来配置。

#### 1.2 设置中文

依次点击左上角的 **Options** - **General settings** 会看到一个 Language 选项，选择中文后重新启动 Cemu 生效。

#### 1.3 初始化 Cemu

- 添加游戏路径

  点击 **选项** - **通用设置** 在游戏路径下方点击 **添加** 按钮，选择一个文件夹如 `D:\Games\WiiUGames`，之后我们会把下载的游戏放在这里。

- 安装图形插件

  依次点击 **选项** - **图形插件** - **下载最新社区图形插件**，下载成功之后关闭弹窗就行。

#### 1.4 连接手柄

首先您需要将手柄连接到电脑，当然也可以用键盘，这里以手柄举例。

点击 **选项** - **输入设置** 进行控制器配置，配置如下：

```
配置文件: 任意配置文件名

模拟控制器: Wii U Pro Controller

控制器:
	API: SDLController
	控制器: Nintendo Switch Pro Controller（下拉框选择时可能会空白 1 秒左右）

```

选择之后可以测试和校准一下。

如果您有设置键盘或者其他问题，请参考网上的教程。





### 2. 使用 WiiUDownloader 下载游戏

推荐使用 [WiiUDownloader](https://github.com/Xpl0itU/WiiUDownloader)，它是目前体验最好的 Wii U 游戏下载器。允许您从任天堂服务器下载 Wii U 游戏。

#### 2.1 安装

你可以从 [WiiUDownloader Release](https://github.com/Xpl0itU/WiiUDownloader/releases) 下载最新的应用程序包并解压到合适的位置，比如 `D:\Games\WiiUDownloader\`。

首次运行 WiiUDownloader 会出现初始化设置弹窗，同样建议你直接点击跳过。

#### 2.2 下载游戏

勾选下载界面的底部的 `Decrypt contents` 和 `Decrypt encrypted Contents afert decryption` 。

仅勾选右下角的 Japan 选项，因为游戏的中文语言包是基于 Japan 版本的。



在搜索栏 输入 Zelda 选择这些项目（看不懂可以用截图翻译）：

Game - Title ID  00050000101c9300 **必须**，这是《塞尔达传说 旷野之息》游戏本体

Update - Title ID 0005000e101c9300 **必须**，这是游戏更新，不下载的话进游戏会提醒需要更新

DLC - Title ID0005000c101c9300 可选。



点击 **Download Queue** 选择之前创建的游戏目录，等待下载完成即可。下载完成后打开 Cemu 就可以看到游戏了。

### 3. 游戏设置中文

#### 3.1 安装中文语言包

点击下载 [塞尔达传说：旷野之息简体中文包](https://github.com/Leskur/cemu-zelda-guide/raw/refs/heads/main/%E5%A1%9E%E5%B0%94%E8%BE%BE%E4%BC%A0%E8%AF%B4%EF%BC%9A%E6%97%B7%E9%87%8E%E4%B9%8B%E6%81%AF%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87%E5%8C%85.zip)，解压后将 **整个文件夹** 放到 Cemu 的图形插件目录，文件夹名称随意。

Windows 路径：`C:\Users\{你的用户名}\AppData\Roaming\Cemu\graphicPacks\`

其他系统自己找一下。



添加后重启 Cemu 可以在图形插件界面找到。

#### 3.2 切换为中文

在 Cemu 的游戏列表找到 Zelda，点击右键 - 编辑图形插件，展开 Zelda 的选项，你会看到 Languages 下有简体中文选项，勾选它即可。

然后启动游戏就是中文语言了，Zelda 启动！

### 4. 游戏优化

#### 帧率提升

直接运行游戏默认会锁定 30FPS，你可以使用 FPS++ 插件提升 FPS 限制

在 Cemu 的游戏列表找到 Zelda，点击右键 - 编辑图形插件找到 The Legend of Zelda: Breath the Wild/Mods/FPS++（你也可以直接搜索 FPS++）。

勾选 FPS++

#### CEMU 优化

其他 Cemu 优化可以参考 [Optimizing Cemu](https://cemu.cfw.guide/optimizing-cemu.html)
