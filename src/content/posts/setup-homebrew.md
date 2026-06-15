---
title: Homebrew 一款开源软件包管理工具
published: 2026-06-15
pinned: false
description: Homebrew 是 macOS 和 Linux 系统上的开源软件包管理工具，可简化软件包的安装、更新、管理过程，被比作 macOS 上的 “开发工具商店”，能通过一行命令安装、更新或卸载软件，如 Node.js、Git、Vim 等。
tags: [开发工具]
category: 开发者
draft: false
image: ./cover_images/bilanhangxian-1.avif
---


## Homebrew

Homebrew 是 macOS 和 Linux 系统上的开源软件包管理工具，可简化软件包的安装、更新、管理过程，被比作 macOS 上的 “开发工具商店”，能通过一行命令安装、更新或卸载软件，如 Node.js、Git、Vim 等。

**安装方式** ：在终端（Terminal）输入命令

```Shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

安装过程中会提示输入开机密码（输入时屏幕不显示字符，输完按回车即可）。若安装进度过慢，请确认已连接 VPN。

**常用命令** ：

| 操作          | 命令                                         |
| ----------- | ------------------------------------------ |
| 安装软件        | `brew install [软件名]` ，如 `brew install git` |
| 卸载一个软件包     | `brew uninstall [软件名]`                     |
| 更新 Homebrew | `brew update`                              |
| 更新所有软件      | `brew upgrade`                             |
| 查看已安装软件     | `brew list`                                |
| 查看版本号       | `brew -v`                                  |
| 搜索可用的软件包    | `brew search <text>`                       |
| 列出所有过时的软件包  | `brew outdated`                            |
| 诊断工具        | `brew doctor`                              |

**安装参考** ：<https://brew.sh/zh-cn/> 。

**官网** ：<https://brew.sh/>

## 扩展：其他包管理工具

1.  **NPM**

**定义** ：NPM（Node Package Manager）是 Node 环境中的包管理器，安装 Node.js 时会自动安装。它提供超过 200 万个包，周下载量超过 1000 亿次，用户可通过一行命令在项目中使用 NPM 中的包 。

**与 Node.js 的关系** ：Node.js 是开源、跨平台的 JavaScript 运行时环境，主流前端框架都依赖 Node.js。安装 Node.js 后会自动安装 NPM 。

**使用示例** ：在 NPM 平台上搜索并安装 shadcn 项目，可使用 `npm i shadcn` 命令，相关页面展示了 shadcn 的版本、依赖项、下载量等信息 。

2.  **WinGet**

**定义** ：WinGet 是 Windows 系统的包管理器，可用于安装、更新软件 。

**与 Claude Code** **的关系** ：可使用 WinGet 安装 Claude Code（Anthropic AI 编程助手命令行工具），但使用 WinGet 安装的版本不会自动更新，需定期手动执行 `winget upgrade Anthropic.ClaudeCode` 来获取最新功能与安全修复 。

## 安装Homebrew

1.  打开终端，输入shell命令

```Shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2.  在任务执行暂停时，根据提示输入设备密码

```Shell
==> Checking for `sudo` access (which may request your password)...
[password:
```

3.  按回车键继续 或 其他人任意键终止(安装任务)

```Shell
Press RETURN/ENTER to continue or any other key to abort:
```

4.  可能的遇到的问题no.1:

```Shell
xcode-select: note: install requested for command line developer tools
Press any key when the installation has completed.
```

这里是因为未安装 `Xcode command-line tool`

会自动弹出安装程序，请在安装完成后按任意按钮继续任务。

![截屏2026-05-09 23.34.32.png](https://p0-xtjj-private.juejin.cn/tos-cn-i-73owjymdk6/f2ccaa3752fe4013879edc339046a126~tplv-73owjymdk6-jj-mark-v1:0:0:0:0:5o6Y6YeR5oqA5pyv56S-5Yy6IEAg5rOh6IqZ5omN5LiN5Lya6ZW_6IOWdw==:q75.awebp?policy=eyJ2bSI6MywidWlkIjoiMzY1OTYxNjAzOTk5ODI0OCJ9&rk3s=f64ab15b&x-orig-authkey=f32326d3454f2ac7e96d3d06cdbb035152127018&x-orig-expires=1782100508&x-orig-sign=uEY94t3siNsrsxmdIUnPGL3NFNc%3D)

关于`Xcode command-line tools`，详见Apple官方文档：<https://developer.apple.com/documentation/xcode/xcode-command-line-tool-reference>

若提示“**不能安装该软件，因为当前无法从软件更新服务器获得**”，则可能是用户的网络和苹果服务器连接不上，就会报错。

可以在调整网络后，再次执行`xcode-select --install`重新安装。

若下载任务始终失败，则有两种解决方案：

*   去Apple官网（ <https://developer.apple.com/download/all/> ），搜索`Command Line Tools for Xcode`下载系统对应版本
*   安装Xcode，安装后，在终端执行 `sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer`，即可使用其命令行工具。

完成后，可运行下面命令检查结果：

| 操作      | 命令                |
| ------- | ----------------- |
| 检查工具路径  | `xcode-select -p` |
| 验证编译器可用 | `clang --version` |

5.  继续安装Homebrew，按提示依次输入

```Shell
==> Next steps:
- Run these commands in your terminal to add Homebrew to your **PATH**:
    echo >> /Users/houyaohui/.zprofile
    echo 'eval "$(/opt/homebrew/bin/brew shellenv zsh)"' >> /Users/houyaohui/.zprofile
    eval "$(/opt/homebrew/bin/brew shellenv zsh)"
```

只需要按提示依次在命令行输入以上命令。

6.  运行`brew doctor`验证安装

## 其他问题

1.  **Xcode**与**CLT**(Command Line Tools)重复

`Command Line Tools`的下载是Homebrew安装中常遇到的问题，因为国内网络问题往往会导致反复尝试。

若本地既下载了 Xcode，又独立下载安装了 CLT；若无iOS开发需要，那么建议移除Xcode以避免干扰。

直接把 Xcode 丢进废纸篓，然后重置工具链指向：

```Shell
sudo rm -rf /Applications/Xcode.app
sudo xcode-select --reset
```

之后 `xcode-select -p` 会回到 `/Library/Developer/CommandLineTools`。
