# 中文说明文档

***English README is in [README_EN.md](README_EN.md)***

## 开源协议

***使用[LGPLv2.1](LICENSE.txt)协议开源***

***请遵守开源协议***

***请遵守开源协议***

## 功能

### 被动技

- 移除视角转动限制
- 修复中文玩家名显示`□`
- 移除玩家名字长度限制（HUD与聊天）
- 移除只能发送小写限制
- 移除敏感词限制（房主需要）

### 主动技

- 疯狂转头
- 张嘴
- 头部移动
- 身体移动
- 身体转动
- 头部前后移动
- 上下移动

#### 按键列表

| 按键               | 功能         |
| :----------------: | :---------: |
| `I`                | 疯狂转头     |
| `O`                | 张嘴         |
| `↑` `↓` `←` `→`    | 头部移动     |
| `鼠标滚轮`          | 头部前后移动 |
| `W` `S` `A` `D`    | 身体移动     |
| `鼠标右键` + `转动` | 身体转动     |
| `LeftShift`        | 上移动       |
| `LeftCtrl`         | 下移动       |
| `Insert`           | 启用移动     |
| `Delete`           | 启用提示     |
| `Home`             | 重置头部     |
| `End`              | 重置身体     |

### 做不到

- 看别人的牌
- 修改手中的牌型
- 不死

## 安装

***如果觉得麻烦，可以尝试一键安装工具[LiarsBarEnhanceInstaller](https://github.com/TianMengLucky/LiarsBarEnhanceInstaller)***

1. 下载[BepInEx](https://github.com/BepInEx/BepInEx/releases/download/v5.4.23.2/BepInEx_win_x64_5.4.23.2.zip)
2. 将`BepInEx`解压至游戏根目录（[官方安装教程](https://docs.bepinex.dev/articles/user_guide/installation/index.html)）
3. 从[Release](https://github.com/dogdie233/LiarsBarEnhance/releases)下载[最新Dll本体](https://github.com/dogdie233/LiarsBarEnhance/releases/download/1.0.0/com.github.dogdie233.LiarsBarEnhance.dll)
4. 将插件本体(`com.github.dogdie233.LiarsBarEnhance.dll`)放置在插件文件夹（即`<游戏根目录>/BepInEx/plugins`）（没有`plugins`文件夹请手动创建）

## 自行构建插件

***Release 会发布构建完成的插件，非必要不建议自行构建***

1. 确保已经安装了[.NET SDK](https://dotnet.microsoft.com/zh-cn/download)（兼容netstandard2.1的SDK如6.0或以上）  
2. `cmd` 或者 `powershell` 等终端输入 `git clone https://github.com/dogdie233/LiarsBarEnhance.git`克隆本仓库到本地(前提安装`Git`网上教程一堆)或点击绿色`code`按钮后点击`Download Zip`下载解压  
3. 设置环境变量`LiarsBarManaged`为`<游戏根目录>/Liar's Bar_Data/Managed/`或者从`<游戏根目录>/Liar's Bar_Data/Managed/`将[列表](#所需复制文件)中的dll文件复制到`lib`文件夹中  
4. 在项目根目录执行`dotnet build -c Release`  
5. 插件本体`com.github.dogdie233.LiarsBarEnhance.dll`将会生成在`Output`目录下  

***按照[安装](#安装)继续进行下一步操作***  

## 所需复制文件

- `Assembly-CSharp.dll`
- `Mirror.dll`
- `UnityEngine.UI`
- `Unity.TextMeshPro.dll`
- `Unity.Localization.dll`

## 其他

欢迎欢愉的功能贡献（影响游戏平衡除外），可以提起功能请求等待有兴趣的开发者实现  
Xiaoye97大佬的BepInEx模组插件基础教程:  
[BepinEx5安装教程【Unity游戏Mod/插件制作教程02 - BepInEx的安装和使用-哔哩哔哩】](https://www.bilibili.com/read/cv8997496/)
