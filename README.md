# Ikemen GO
IKEMEN Go is a remake of the IKEMEN (open source fighting games engine that supports M.U.G.E.N resources) in Google’s Programming Language “Go”.

IKEMEN Go 是 使用Go语言对IKEMEN的重制版本
## Installing 安装
Ready to use builds for Windows, MacOS and Linux can be found on the releases tab of the repo. 

windows, macOS以及linux的可用构建版本可在release页找到
## Running 运行
On windows, execute `Ikemen_GO.exe` (`Ikemen_GO_x86.exe` on 32-bit OS)  
On MacOS or Linux, double-click on `Ikemen_GO.command`

在windows系统下, 执行Ikemen_GO.exe  
在MacOS或者linux系统下, 双击Ikemen_go.command

## Developing 开发
These instructions are for those interested in developing the Ikemen_GO engine. Instructions on contributing with custom stages, fonts, characters and other resources can be found in the community forum.

这些说明适用于那些有兴趣开发Ikemen_GO引擎的人。有关使用自定义阶段、字体、字符和其他资源进行贡献的说明，请参阅社区论坛。
### Building on Windows windows下构建
Check the instructions [here](https://github.com/ikemen-engine/Ikemen-GO/wiki/Building-on-Windows)

### Building on Mac    Mac下构建
Check the insturctions [here](https://github.com/ikemen-engine/Ikemen-GO/wiki/Building-on-MacOS)

### Building on Linux  Linux下构建
Check the instructions [here](https://github.com/ikemen-engine/Ikemen-GO/wiki/Building-on-Linux)

### Debugging 调试
Download the [Mugen dependencies](https://github.com/ikemen-engine/Ikemen_GO-Elecbyte-Screenpack) and unpack them into the Ikemen-GO source directory.
Then, use [Goland](https://www.jetbrains.com/go/) or [Visual Studio Code](https://code.visualstudio.com/) to debug.

下载[Mugen dependencies](https://github.com/ikemen-engine/Ikemen_GO-Elecbyte-Screenpack) 并解压到项目source目录, 然后使用goland或者vscode进行调试
### Cross-compiling binaries with docker (Linux/Windows/MacOS) 使用docker进行交叉编译
The easiest way to compile binaries for other platforms is with Docker.  
You don't need the native development environment set to be able to build binaries if you decide to use Docker.  
The image downloaded has all required tools to compile Ikemen_GO for all the three platforms.

为其他平台编译二进制文件最简单的方式是使用docker.  
如果你决定使用docker 你不需要原生开发环境  
下载的镜像已经包括了编译Ikemen_GO到全部三种平台的所有工具

Install [docker for your platform](https://www.docker.com/get-started).  
For MacOS, you can install using homebrew (`brew cask install docker`).

选择对应的平台安装docker  
对于MacOS, 你可以使用homebrew安装

Open a terminal, go to Ikemen `build` directory folder and then run the script `build_docker.sh`.  
Look inside the script for details on how it works.

打开终端, 进入Ikemen `build` 目录然后执行`build_docker.sh`  
关于它如何工作可以查看脚本的细节

### Preparing for release  准备发行
Before generating the installation bundle, first make sure that the binaries for Ikemen_GO are properly generated.  
Download and install [InstallBuilder](https://installbuilder.bitrock.com).  
Once finished, open the program, then open the file releaseconf.xml.  
Click in Build.  
For other platforms, select the target platform then click in build.

在生成安装包之前, 首先确保Ikemen_GO的二进制文件已经生成.  
下载并安装InstallBuilder  
安装完成后, 打开程序, 然后打开文件 `releaseconf.xml`
点击Build  
如果需要修改模板平台, 选择目标平台然后进行构建


You may edit releaseconf.xml or use the InstallBuilder wizard to customize the installer.  
你可能需要修改releaseconf.xml或者使用InstallBuilder向导来自定义安装包  

NOTE: InstallBuilder is free for opensource projects. But you need to [get a license for it](https://installbuilder.bitrock.com/open-source-licenses.html).  
Do not include copyrighted dependencies in the bundle.  
注意: InstallBuilder作为开源软件是免费的, 但是你需要获得license  
不要在包体中包含有版权的依赖

## Features added since Mugen  
Refer to the wiki article [Details of new features](https://github.com/ikemen-engine/Ikemen-GO/wiki) to see new features added that are not available in Mugen 1.1 and bellow.

## References
Suehiro repo (Original creator of the engine)  
https://osdn.net/users/supersuehiro/pf/ikemen_go/

Ikemen GO, K4thos fork of Ikemen. (Commonly updated and merged constantly to this repo)  
https://github.com/K4thos/Ikemen-GO-Plus

The default motif bundled with the engine:  
https://github.com/ikemen-engine/Ikemen_GO-Elecbyte-Screenpack

## What I.K.E.M.E.N means.  I.K.E.M.E.N是什么意思?
Ikemen is an acronym of:  
Ikemen是一个缩写

**い**つまでも **完**成しない **永**遠に **未**完成 **エン**ジン  
**I**tsu made mo **K**ansei shinai **E**ien ni **M**ikansei **EN**gine  
尚未完成的永不完成的引擎

## Licence  协议
The code is under the MIT Licence.  
Non-code assets are under CC-BY 3.0.  
代码遵守MIT协议  
非代码资产遵守 CC-BY 3.0

Check [License.txt](License.txt) for more deatils.  
更多细节请查看 [License.txt](License.txt)
