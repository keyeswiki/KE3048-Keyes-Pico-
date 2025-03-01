# Python 教程 Windows

## 开发环境设置

在开始构建项目之前，你需要首先做一些准备，这是非常重要的，你不能跳过。

1.  安装Thonny(重要)

Thonny是一个免费、开源的软件平台，体积小，界面简单，操作简单，功能丰富，是一个适合初学者的Python     IDE。在本教程中，我们使用这个IDE在整个过程中开发树莓派Pico。Thonny支持多种操作系统，包括Windows,     Mac OS, Linux。

1.  下载Thonny软件

(1)进入软件官网：[<u>https://thonny.org</u>](https://thonny.org)下载Thonny软件，最好下载最新版的，否则可能不支持树莓派
Pico.

(2)Thonny的开源代码库：[<u>https://github.com/thonny/thonny</u>](https://github.com/thonny/thonny)

请按照官网的指导安装或点击下面的链接下载安装。(请根据您的操作系统选择相应的选项.)

|操作系统|下载链接/方法|
|-|-|
|MAC OS：|[https://github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.pkg](https://github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.pkg)|
|Windows：|[https:/github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.exe](https://github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.exe)|
|Linux：|最新版本: Binary bundle for PC (Thonny+Python): bash <(wget -O - https://thonny.org/installer-for-linux) With pip: pip3 install thonny Distro packages (may not be the latest version): Debian, Rasbian, Ubuntu, Mint and others: sudo apt install thonny Fedora: sudo dnf install thonny|

![](media/bd5823ede2c01d1fa4696438c62aec51.png)

2.  在Windows上安装Thonny软件

1.  下载后的Thonny图标如下。

![](media/d3caa98d406fa06a124d5c98195b90db.png)

2.  双击“thonny-3.3.13.exe”，会出现下面对话框，我这里是选择“![](media/11fb59a50abe0bf54df7e4cb891ad2c0.png)”进行操作的。你也可以选择“![](media/37be3f3bcc9aa0eb48c8b844eb46a71c.png)”进行操作的。

![](media/4c044b255da8b14fe674eb9cce01627d.png)

3.  如果您不熟悉电脑软件安装，您可以一直单击“Next”直到安装完成。

![](media/995b36640124b6a9b23f10473ff8a38a.png)

![](media/8bcc17840b9fc15d76f79fee8a0168ee.png)

4.  如果您需要更改Thonny软件的安装路径，可以单击“Browse...”进行修改。选择安装路径后，单击“OK”。

如果您不想更改安装路径，只需单击“Next”；然后又继续单击“Next”。

![](media/df6f63b42ebb1676b22c26b25dc9c7aa.png)

![](media/f5cd6d619b4645601c5b098ffdbec12a.png)

5.  选中“Create desktop     icon”，Thonny软件会在你的桌面上生成一个快捷方式，方便你稍后打开Thonny软件。

![](media/a30c89dde3de81ad00aced30510071be.png)

6.  单击“Install”安装软件。

![](media/6ace65142291e5e8af5f81e4a6b2f180.png)

7.  在安装过程中，您只需等待安装完成，千万不要点击“Cancel”，否则将无法安装成功。

![](media/a504b3a3ab16b4d91040cd5878acea0c.png)

8.  一旦看到如下界面，就表示已经成功安装了Thonny软件，点击“Finish”就可以。

![](media/a1fb6027e54a975de1c0aa1e1a0d6a29.png)

9.  如果你在安装过程中选择了“Create desktop     icon”，则可以在桌面上看到如下图标。

![](media/80f35044d91d66f734e36059db35f273.png)

2.  Thonny软件基本配置

1.  双击Thonny软件的桌面图标，可以看到如下界面，同时还可以进行语言选择(这里选择简体中文)和初始设置。设置完了点击“Let’s     go！”。

![](media/ee240978a4f844184f1ea9f5a21d0395.png)

![](media/bfb4c5bdce61fdd384c32afb17ba9145.png)

![](media/fb2631689bfa02c2476fb12e16f7cd16.png)

![](media/ec56f1d21d0e2010d306acb9195228f8.png)

![](media/6191607fb74b8b2678742c6e341c5454.png)

2.  选择“视图”→“文件”和“Shell”。

![](media/0d7f11d612c0fbfcf7e585996035144f.png)

![](media/0e7fe35efdb4437a25fe5ed6532305a7.png)

![](media/3e08de0701a8c9e6686f3545f33be67d.png)

3.  更新Micropython固件（重要）

要在树莓派Pico板上运行MicroPython程序，我们需要先烧入一个固件到树莓派Pico板中。

1.  为什么我们需要更新固件

树莓派Pico板可以用C语言和MicroPython语言编程，并且树莓派Pico板出厂时没有MicroPython固件，使用MicroPython编程之前需要下载MicroPython固件。

注意：MicroPython固件只需要下载一次，当使用MicroPython编程时不需要再次下载。如果你已经下载了用C语言编写的 .uf2
程序固件，则MicroPython固件将会被覆盖，那下次你使用MicroPython时，你需要按照以下步骤更新树莓派Pico板的固件。

2.  下载Micropython固件

方法1：树莓派Pico的官网：[<u>https://www.raspberrypi.com/documentation/microcontrollers/</u>](https://www.raspberrypi.com/documentation/microcontrollers/)

1.  单击上面的链接，你可以看到以下界面：

![](media/3b3e6a639416b76c44f2a0854dc451cc.png)

2.  滚动鼠标，你又可以看到以下内容：

![](media/5d04d67506852588d126ce760739a3c5.png)

3.  单击“MicroPython(Getting started     MicroPython)”进入固件下载页面。

![](media/e8d9658a60f750a654bd2d7a98fe3bb5.png)

方法2：通过单击下载链接：[<u>https://micropython.org/download/rp2-pico/rp2-pico-latest.uf2</u>](https://micropython.org/download/rp2-pico/rp2-pico-latest.uf2)，可以直接下载。

方法3：如果你因为网络问题或其他原因无法下载，可以使用我们准备的 .uf2
文件，它位于以下文件路径

![](media/fe7933eaf8947f37d71b2ee220f43f68.png)

3.  烧入MicroPython固件的步骤

①连接microUSB线一端到你的电脑USB口。

②长按“树莓派Pico板”上的白色按钮（BOOTSEL）。然后，通过microUSB线另一端将树莓派Pico板与电脑连接。

![](media/33c91d51b2aeb2c943691706354aaad1.png)

③松开按钮，当连接成功时，在你的电脑上打开\[设备管理器\]，电脑将自动识别可移动磁盘(RPI-RP2)，如下所示:

![](media/87e24af3ea812b5492a06b0141060b86.png)

④复制文件（rp2-pico-20210902-v1.17.uf2）到可移动磁盘(RPI-RP2)，并等待它完成，就像复制文件到U盘一样。

![](media/8c218b13da74eb39b53a4c27772606a4.png)

![](media/abced882bd94c171759c43b4c5f73215.png)

⑤当固件烧入完成后，树莓派Pico板会自动重启。之后，你可以运行Micropython。

四、Thonny软件连接上树莓派Pico板

1.打开Thonny软件，点击“运行”并选择“选择解释器…”

![](media/b3fe23f5d4dda9dd3d9253c2434b7789.png)

3.  选择“Micropython (一般)”或“Micropython (Raspberry Pi     Pico)”均可。如何选择“Micropython(Raspberry Pi Pico)”?
如下所示：

![](media/c746f079db6a1e174371b3e8e123b08c.png)

3.选择“USB-SERIAL (COMx)”，“COMx”的编号在不同的电脑之间可能会有所不同。你只需要确保选择“USB-SERIAL (COMx)”就行。

如何确定你的树莓派Pico板与电脑通信的端口?

步骤1:当你的树莓派Pico板没有连接到电脑时，打开Thonny软件，点击“运行”，选择“选择解释器...”，弹出对话框，点击“端口”，可以查看当前连接的端口，如下图所示:

![](media/b54aba987917cb42fe6a6266b61e3d0b.png)

步骤2:关闭对话框。将树莓派Pico板连接到电脑，再次单击“运行”并选择“选择解释器...”。单击弹出窗口中的“端口”，查看当前端口。现在又增加了一个端口，那么这个端口是用来与电脑通信的。

![](media/8001573d8beb85a0b8fc2b3adb724ce5.png)

4.  选择“Micropython(Raspberry Pi Pico)”和端口后，单击“确定”。

![](media/5ef3eeaabb007608ab6d88863d7c6bfa.png)

5.  当在Thonny软件上显示以下消息时，表明Thonny软件已成功连接到树莓派Pico板。

![](media/dc3f41145dc9bb38578e0d47cbeb85c7.png)

到目前为止，所有的准备工作都已就绪。

五、测试代码(重要)

1.测试Shell命令

在“Shell”窗口输入“print(Hello World!)”，按“Enter”键。

![](media/237c688f1fd26050fc66c824bab2351e.png)

2.在线运行代码：

要在线运行树莓派Pico，你需要把树莓派Pico板连接到电脑上。这样就可以使用Thonny软件编译或调试程序。

优点：（1）你可以使用Thonny软件编译或调试程序。

（2）通过“Shell”窗口，你可以查看程序运行过程中产生的错误信息和输出结果，并可以在线查询相关功能信息，帮助改进程序。

缺点：（1）要在线运行树莓派Pico，你必须将树莓派Pico板连接到一台电脑上并和Thonny软件一起运行。

（2）如果树莓派Pico板与电脑断开连接，当它们重新连接时，程序将无法再次运行。

基本操作：

（1）打开Thonny软件，并且单击![](media/6388aa0daa514f9325fb07fd5ab6749b.png)“打开...”。

![](media/ad92605d73ff032633997e889b5a8d12.png)

（2）在新弹出的窗口中，点击“此电脑”。

![](media/4a648e13d503cef0dad076d295eeff7e.png)

在新的对话框中，进入文件夹2. 项目教程\项目 01：Hello World选中“Project_01_HelloWorld.py”,单击“Open”。本教程中使用的代码保存在“3. Python 教程\1. Windows 系统\2.项目课程”中。你可以把代码移到任何地方。例如，我们将“2.项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

![](media/b96b7318b5a7424943a921579df1f9e0.png)

（3）单击![](media/f79b2c42507d12b91ca23ea0bb87c5c2.png)“运行当前脚本”来执行程序“Hello World!”, "Welcome keyes" 将打印在“Shell”窗口。

![](media/4bd8b5e357fd0add80c33d6d754bbb19.png)

退出在线运行

当在线运行时，单击Thonny软件上的![](media/fee1916cdaf53677f5117fbc5b65f4cf.png)“停止
/重启后端进程”或按Ctrl+C退出程序。

![](media/780ca09b2d54377ea8f6effc00897d97.png)

3.离线运行代码：

在离线运行时，树莓派Pico板不需要连接电脑和Thonny软件。一旦上电，它就可以运行存储在树莓派Pico板中的main.py程序。

优点：不需要连接电脑和Thonny软件就可以运行程序。

缺点：出现错误或树莓派Pico板没电时，程序会自动停止，并且代码不容易更改。

基本操作：

一旦上电后，树莓派Pico板会自动检查设备上是否存在main.py。如果有，则运行main.py中的程序，然后进入shell命令系统。(如果你想让代码离线运行，你可以将它保存为main.py);
如果main.py不存在，则直接进入shell命令系统。

（1）单击 “文件”→“新文件” 创建并编写代码。

![](media/a37e32734e9502db5706d851c355c71d.png)

（2）在新打开的文件中输入代码。这里我们以Project_02_Onboard_LED_flashing.py代码为例。

![](media/5072bd0f2c59626f7e8f98d09eca3eef.png)

（3）单击菜单栏上的![](media/861d55963959682fdb0ffe4b7f892fe1.png)“保存”,你可以将代码保存到此电脑或Raspberry Pi Pico。

![](media/29b86c444510a311984f20f59b0dea48.png)

4.  选择“Raspberry Pi     Pico”，在新弹出的窗口中输入“main.py”并单击“确认”。

![](media/0e3056c5c3875a0e87fb909ce36c5646.png)

![](media/2d3e53ef359ac655530856974e2401a2.png)

5.  你可以看到代码已经被上传到树莓派Pico板。

![](media/8d45642e75bf678789085198bde01511.png)

（6）断开树莓派Pico板的microUSB线，再重新连接，树莓派Pico板上的LED会反复闪烁。

![](media/e12ecf9006915a143134d18d53643ee4.png)
![](media/6f49241878e04e8ba4edd30fb2714249.png)

0.5秒

退出离线运行

连接树莓派Pico板到电脑，点击Thonny软件上的![](media/9994536062b2b521a194db65bbea995e.png)“停止/重启后端进程”结束离线运行。

![](media/ec2eccd60ec3e4aef89e3bacc957cc59.png)

如果它不能工作，请点击Thonny软件上的![](media/9994536062b2b521a194db65bbea995e.png)“停止/重启后端进程”多次或重新连接树莓派Pico板。

![](media/d08f1eefc580f16a910ae5ad89384bac.png)

我们提供了一个main.py文件用于离线运行。添加到main.py中的代码是执行用户代码文件的引导程序。你只需要将离线项目的代码文件(.py)上传到“Raspberry Pi Pico”。

①将程序文件夹“3. Python 教程\1. Windows 系统\2.项目课程”提前移动到Disk(D)，路径为D:\2.项目课程。打开Thonny软件。

![](media/a0c1aa26b839eeeef53415bf63575d33.png)

②在Disk(D)目录下D:\\2.项目课程中展开“项目00：main”，鼠标左键双击main.py，我们提供的main.py可以使“Raspberry Pi Pico”中的代码离线运行。

![](media/9352c8987212ae2fadabaccd93b237d1.png)

这里，我们使用项目 00和项目02案例作为演示。使用树莓派Pico板上的LED（GP25引脚）显示结果。如果你已经修改了Project_02_Onboard_LED_flashing.py文件，那么你需要相应地修改它。如下图所示，鼠标右键单击Project_02_Onboard_LED_flashing.py文件，选择“上载到/“上传代码到 Raspberry Pi Pico。

![](media/2e2bf285eba09bae4d50e4affaddc379.png)

用同样的方法上传main.py

![](media/3dec40f745ec0103908a7e24dc7d5143.png)

![](media/b2cb646ac79b1b0da4e8ed9bd0b54b48.png)

断开树莓派Pico板的microUSB线并重新连接，树莓派Pico板上的LED将反复闪烁。

![](media/e12ecf9006915a143134d18d53643ee4.png)
![](media/6f49241878e04e8ba4edd30fb2714249.png)

0.5秒

注意:

这里的代码是离线运行的。如果你想停止离线运行并且在“Shell”窗口显示对应信息，只需单击Thonny软件上的![](media/9994536062b2b521a194db65bbea995e.png)“停止/重启后端进程”。

![](media/37adb2c653f32aff1430d84b57ef1420.png)

六、Thonny常见的操作

上传代码至Raspberry Pi Pico

在Project 01：Hello World文件夹中，鼠标右键单击选中Project_01_HelloWorld.py，选择“上载到/”上传代码到Raspberry Pi Pico的根目录。

![](media/95686a19321bb411ab4a5b6ba078c997.png)

下载代码至电脑

在“Raspberry Pi Pico”中，鼠标右键单击选中Project_01_HelloWorld.py，选择“下载到/”将代码下载到你的电脑。

![](media/5360cc2e106c0cb14bb2da87e53c2f68.png)

删除Raspberry Pi Pico根目录中的文件

在“Raspberry Pi Pico”中，鼠标右键单击选中Project_01_HelloWorld.py，选择“删除”，从Raspberry Pi Pico根目录中删除Project_01_Hello World.py。

![](media/44eef0acff104423cb7d4afeade6e92d.png)

删除电脑目录中的文件

在Project 01：Hello World文件夹中，鼠标右键单击选中Project_01_HelloWorld.py，选择“移动到回收站”，即可从Project 01：Hello World文件夹中删除。

![](media/70f40ec3fe52a7f1e27728f26b3ae763.png)

创建和保存代码

（1）单击 “文件”→“新文件” 创建并编写代码。

![](media/a37e32734e9502db5706d851c355c71d.png)

（2）在新打开的文件中输入代码。这里我们以Project_02_Onboard_LED_flashing.py代码为例。

![](media/5072bd0f2c59626f7e8f98d09eca3eef.png)

（3）单击菜单栏上的![](media/861d55963959682fdb0ffe4b7f892fe1.png)“保存”,你可以将代码保存到此电脑或Raspberry Pi Pico。

![](media/29b86c444510a311984f20f59b0dea48.png)

6.  选择“Raspberry Pi Pico”，在新弹出的窗口中输入“main.py”并单击“确认”。

![](media/0e3056c5c3875a0e87fb909ce36c5646.png)

![](media/2d3e53ef359ac655530856974e2401a2.png)

7.  你可以看到代码已经被上传到Raspberry Pi Pico。

![](media/8d45642e75bf678789085198bde01511.png)

⑥单击![](media/abd47da3d3d7e2e2acd2d8fa46397c95.png)“当前运行脚本”,树莓派Pico板上的LED会周期性闪烁。

![](media/009ff6bec53ab149447bdd0d708fc890.png)






## 项目课程

### 项目 01: Hello World

1.项目介绍：

对于树莓派Pico初学者，我们将从一些简单的东西开始。在这个项目中，你只需要一个树莓派Pico板，USB线和电脑就可以完成“Hello World!”项目。它不仅是树莓派Pico和电脑的通信测试，也是树莓派Pico板的初级项目。

2.项目元件：

|![](media/8ea81d60b8e2132c358041235490b7d5.jpeg)|![](media/3bdcc62cfa661d2b860a76e28537e21e.png)|
|-|-|
|树莓派Pico板*1|USB 线*1|

3.项目接线：

在本项目中，我们通过USB线将树莓派Pico板和电脑连接起来。连接方法请参照文档：开发环境设置

![](media/bbebdf7f2c0f4c223b6f2548d7ff6607.png)![](media/8ea81d60b8e2132c358041235490b7d5.jpeg)

4.在线运行代码：

要在线运行树莓派Pico，你需要把树莓派Pico板连接到电脑上。这样就可以使用Thonny软件编译或调试程序。

优点：1. 你们可以使用Thonny软件编译或调试程序。

2. 通过“Shell”窗口，你们可以查看程序运行过程中产生的错误信息和输出结果，并可以在线查询相关功能信息，帮助改进程序。

缺点：1.要在线运行树莓派Pico，你必须将树莓派Pico板连接到一台电脑上并和Thonny软件一起运行。

2.如果树莓派Pico板与电脑断开连接，当它们重新连接时，程序将无法再次运行。

基本操作：

1.打开Thonny软件，并且单击![](media/6388aa0daa514f9325fb07fd5ab6749b.png)“打开...”。

![](media/ad92605d73ff032633997e889b5a8d12.png)

2.在新弹出的窗口中，点击“此电脑”。

![](media/4a648e13d503cef0dad076d295eeff7e.png)

在新的对话框中，选中“Project_01_HelloWorld.py”,单击“Open”。本教程中使用的代码保存在“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

![](media/b96b7318b5a7424943a921579df1f9e0.png)

3.单击![](media/f79b2c42507d12b91ca23ea0bb87c5c2.png)“运行当前脚本”来执行程序“Hello World!”, "Welcome keyes" 将打印在“Shell”窗口。

![](media/4bd8b5e357fd0add80c33d6d754bbb19.png)

退出在线运行

当在线运行时，单击Thonny软件上的![](media/fee1916cdaf53677f5117fbc5b65f4cf.png)“停止
/重启后端进程”或按Ctrl+C退出程序。

![](media/780ca09b2d54377ea8f6effc00897d97.png)

### 项目 02：板载灯闪烁

1.项目介绍：

树莓派Pico板上有个板载LED，这个LED是固定接在树莓派Pico板上的GP25引脚，在这个项目中，我们将来学习使板载LED闪烁的效果。

2.项目元件：

|![](media/8ea81d60b8e2132c358041235490b7d5.jpeg)|![](media/3bdcc62cfa661d2b860a76e28537e21e.png)|
|-|-|
|树莓派Pico板*1|USB 线*1|

3.项目接线：

在本项目中，用USB线将树莓派Pico板和电脑连起来。连接方法请参照文档：开发环境设置

![](media/bbebdf7f2c0f4c223b6f2548d7ff6607.png)![](media/8ea81d60b8e2132c358041235490b7d5.jpeg)

4.项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

代码在线运行：

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
02：板载灯闪烁”。

![](media/f53af2742508818b162febd58c9ba562.png)

展开文件夹“项目
02：板载灯闪烁”，鼠标左键双击“Project_02_Onboard_LED_flashing.py”打开它。如下图所示：

![](media/a3b8f54b674a35e3ec2d83f2d0a49749.png)

确保树莓派Pico板已经连接到电脑上。单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/启动后端进程”，然后去看看“Shell”窗口将显示什么界面。

![](media/05b8bf9eb30a53d49d52e2c4e0eb3758.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：树莓派Pico板的LED开始闪烁。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/启动后端进程”退出程序。

![](media/68f650b2ac69c4f4cc8b088a355a7d35.png)

![](media/e12ecf9006915a143134d18d53643ee4.png)
![](media/6f49241878e04e8ba4edd30fb2714249.png)

0.5秒

注意：这是在线运行的代码。如果你断开USB线，重新启动“Raspberry Pi Pico”，树莓派Pico板上的LED停止闪烁。在Thonny软件“Shell”窗口将显示如下信息：

![](media/c1cc0a84752700e07fc401cff599b364.png)

代码离线运行（上传代码到Raspberry Pi Pico）：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/启动后端进程”。

![](media/f17b6ad78c63483220b262f12218591b.png)

如下图所示，鼠标右键单击文件“Project_02_Onboard_LED_flashing.py”，选择“上载到/”上传代码到Raspberry Pi Pico。

![](media/bfa21cca01279baeb0bee57e43a7a8bb.png)

用同样的方法上传main.py

![](media/248fb7bcb11c59053f6dff467bf000f1.png)

![](media/637b392f746c91c9b46f5fb9fad069a0.png)

断开树莓派Pico板上的USB线并重新连接，树莓派Pico板的LED会反复闪烁。

![](media/e12ecf9006915a143134d18d53643ee4.png)
![](media/6f49241878e04e8ba4edd30fb2714249.png)

0.5秒

注意：这里的代码是离线运行的。如果你想停止离线运行并且在“Shell”窗口显示对应信息，只需单击Thonny软件中的![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/启动后端进程”。

![](media/dd098f448a5c0f0a4209f6b102893289.png)

### 项目 03：外接灯闪烁 

1.  项目介绍：

在这个项目中，我们将向你展示外接LED闪烁效果。我们使用树莓派Pico板的数字引脚打开LED，让它闪烁。

2.  项目元件：

|![](media/6046d0c7d3a11a080a2de23b1969804e.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|公对母杜邦线若干|USB 线*1|
|![](media/7eb361d680dfa351f07f8527aeb37abd.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)||
|红色LED*1|220Ω电阻*1|面包板*1||

3.  元件知识：

（1）LED:

![](media/081141eed6146deed2bfbd8e55a8465b.jpeg)

LED是一种被称为“发光二极管”的半导体，是一种由半导体材料(硅、硒、锗等)制成的电子器件。它有正极和负极。短腿为负极，接GND，长腿为正极，接3.3V或5V。

![](media/14a84d5f016d7566151a5563c502787e.png)

（2）五色环电阻

电阻是电路中限制或调节电流流动的电子元件。左边是电阻器的外观，右边是电阻在电路中表示的符号。电阻(R)的单位为欧姆(Ω)，1 mΩ= 1000 kΩ，1kΩ= 1000Ω。

![](media/8a86f65cf820d08e8956daa70d1c4195.jpeg)
![](media/f6079fe22518f0fc1b0c3a3b93a516a1.png)

我们可以使用电阻来保护敏感组件，如LED。电阻的强度（以Ω为单位）用小色环标记在电阻器的主体上。每种颜色代表一个数字，你可以用电阻对照卡查找。

\-色带1 – 1st Digit.

-色带 2 – 2nd Digit.

-色带 3 – 3rd Digit.

-色带 4 – Multiplier.

-色带 5 – Tolerance.

![](media/c3df005312cd9f6d4cdae6abf3cddb83.png)

在这个套件中，我们提供了3个具有不同电阻值的五色环电阻。这里以3个五色环电阻为例：

220Ω 电阻*10

![](media/793740d0b936e516ca354111e2d0eb79.png)

10KΩ 电阻*10

![](media/18484e5d16b6d89c63825cc2efa6a543.png)

1KΩ 电阻*10

![](media/8088ed382616afb346d44f5aacfb52d1.png)

在相同的电压下，会有更小的电流和更大的电阻。电流(I)、电压(U)、电阻(R)之间的联系可以用公式表示：I=U/R。在下图中，假如电压为3V，则通过R1的电流:
I = U / R = 3 V / 10 KΩ= 0.0003A= 0.3mA。

![](media/b3eec552e4dfad361833730698621776.png)

不要把电阻值很低的电阻直接连接在电源两极，这样会使电流过高而损坏电子元件。电阻是没有正负极之分。

（3）面包板

面包板是实验室中用于搭接电路的重要工具。面包板上有许多孔，可以插入集成电路和电阻等电路元件。熟练掌握面包板的使用方法是提高实验效率，减少实验故障出现几率的重要基础之一。下面就面包板的结构和使用方法做简单介绍。一个典型的面包板如下所示：

![](media/837cd6ec4b1b09cc46340201a6425958.jpeg)

面包板的外观和内部结构如上图所示，常见的最小单元面包板分上、中、下三部分，上面和下面部分一般是由一行或两行的插孔构成的窄条，中间部分是由中间一条隔离凹槽和上下各5
行的插孔构成的条。

![](media/099510035abc223273495e042a7bd6b6.jpeg)

在面包板的两个窄条分别有两行插孔，两行之间是不连通的，一般是作为电源引入的通路。上方第一行标有“+”的一行有10组插孔（内部都是连通），均为正极；上方第二行标有“-”的一行有10组插孔，（内部都是连通），均为接地。面包板下方的第一行与第二行结构同上。如需用到整个面包板，通常将“+”与“+”用导线连接起来，“-”与“-”用导线连接起来。

　　中间部分宽条是由中间一条隔离凹槽和上下各5
行的插孔构成。在同一列中的5
个插孔是互相连通的，列和列之间以及凹槽上下部分则是不连通的。外观及结构如下图：

![](media/3fc9a04d9354e63ca0e89eb7ed627128.png)

中间部分宽条的连接孔分为上下两部分，是面包板的主工作区，用来插接原件和跳线。在同一列中的5个插孔（即a-b-c-d-e，f-g-h-i-j）是互相连通的；列和列之间以及凹槽上下部分是不连通的。在做实验的时候，通常是使用两窄一宽组成的小单元，在宽条部分搭接电路的主体部分，上面的窄条取一行做电源，下面的窄条取一行做接地。中间宽条用于连接电路，由于凹槽上下是不连通的，所以集成块一般跨插在凹槽上。

（4）keyes 树莓派Pico板的扩展板使用方法

将树莓派Pico板堆叠在扩展板上即可使用，如下图：

![](media/027bcb15b34415d54164c03a796a10ab.jpeg)

（5）电源

在本项目中，用USB线将树莓派Pico板和电脑连起来。连接方法请参照文档：开发环境设置

![](media/bbebdf7f2c0f4c223b6f2548d7ff6607.png)![](media/8ea81d60b8e2132c358041235490b7d5.jpeg)

4.  项目电路图和接线图：

首先，切断树莓派Pico板的所有电源。然后根据电路图和接线图搭建电路。电路搭建好并验证无误后，用USB线将树莓派Pico板连接到电脑上。注意：避免任何可能的短路(特别是连接3.3V和GND)!

警告：短路可能导致电路中产生大电流，造成元件过热，并对硬件造成永久性损坏。

![](media/cb069d7553d861e3293d8bdbe85bbd05.png)

电路图

![](media/96800765a20d72653a8cd4a9ae12b636.png)

接线图

注意: 怎样连接LED

![](media/14a84d5f016d7566151a5563c502787e.png)

怎样识别五色环220Ω电阻

![](media/793740d0b936e516ca354111e2d0eb79.png)

5.  项目代码：

根据电路图，当树莓派Pico板的GP16输出高电平时，LED点亮；当输出低电平时，LED灯关闭。因此，我们可以通过控制GP16重复输出高低电平，使LED反复闪烁。

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

代码在线运行：

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
03：外接灯闪烁”。

![](media/9d3a70645a76662b9667ef20536921af.png)

展开文件夹“项目
03：外接灯闪烁”，鼠标左键双击“Project_03_External_LED_flashing.py”打开它。如下图所示：

![](media/99e99a1b595e0cd523a8cbe27351fdef.png)

确保树莓派Pico板已经连接到电脑上。单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”，然后去看看“Shell”窗口将显示什么界面。

![](media/b9ab19cee933429fe9f424013b2b1daa.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，电路中的LED开始闪烁。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/66f948b4a86f73bf9f3efc4912585878.png)

![](media/77dec960e108229b6d97b4af9a2db902.png)
![](media/2dcc6a55b77b4175b5175f717eb196c3.png)

0.5秒

注意：这是在线运行的代码。如果断开USB线，重新启动“Raspberry Pi Pico”，LED停止闪烁。在Thonny软件的“Shell”窗口将显示如下信息：

![](media/b33a2b0093d918581f7e5c3ac98fbef7.png)

代码离线运行（上传代码到Raspberry Pi Pico）：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/66456686dccbd3b5cf836482ea384afe.png)

如下图所示，鼠标右键单击文件“Project_03_External_LED_flashing.py”，选择“上载到/”上传代码到Raspberry Pi Pico。

![](media/4c417c530505c8cd8ff08d8293a8e887.png)

用同样的方法上传main.py

![](media/cb3207aed5ee3d482ee8ca6ff4522a94.png)

![](media/99987126f02784f3d3a067a96b0890f9.png)

断开树莓派Pico板上的USB线并重新连接，电路中的LED会反复闪烁。

![](media/77dec960e108229b6d97b4af9a2db902.png)
![](media/2dcc6a55b77b4175b5175f717eb196c3.png)

0.5秒

注意：这里的代码是离线运行的。如果你想停止离线运行并且在“Shell”窗口显示对应信息，只需单击Thonny软件中的![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/3c11b930b665a45612460c314af455d8.png)

### 项目 04: 呼吸灯

1.项目介绍：

在之前的研究中，我们知道LED有亮/灭状态，那么如何进入中间状态呢?如何输出一个中间状态让LED“半亮”?这就是我们将要学习的。呼吸灯，即LED由灭到亮，再由亮到灭，就像“呼吸”一样。那么，如何控制LED的亮度呢?我们将使用树莓派Pico板的PWM来实现这个目标。

2.项目元件：

|![](media/6046d0c7d3a11a080a2de23b1969804e.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|公对母杜邦线若干|USB 线*1|
|![](media/7eb361d680dfa351f07f8527aeb37abd.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)||
|红色LED*1|220Ω电阻*1|面包板*1||

3.元件知识：

![](media/6549bdbfd4e7b6b2b341012105d655e8.png)

Analog & Digital

模拟信号在时间和数值上都是连续的信号。相反，数字信号或离散时间信号是由一系列数字组成的时间序列。生活中的大多数信号都是模拟信号。一个熟悉的模拟信号的例子是，全天的温度是如何不断变化的，而不是突然从0到10的瞬间变化。然而，数字信号的值可以瞬间改变。这个变化用数字表示为1和0(二进制代码的基础)。如下图所示，我们可以更容易地看出它们的差异。

![](media/4bdf6127e563b453a1fd8953b4ebb277.png)

在实际应用中，我们经常使用二进制作为数字信号，即一系列的0和1。由于二进制信号只有两个值(0或1)，因此具有很大的稳定性和可靠性。最后，可以将模拟信号和数字信号相互转换。

PWM：

脉宽调制(PWM)是一种利用数字信号控制模拟电路的有效方法。普通处理器不能直接输出模拟信号。PWM技术使这种转换(将数字信号转换为模拟信号)非常方便。PWM技术利用数字引脚发送一定频率的方波，即高电平和低电平的输出，交替持续一段时间。每一组高电平和低电平的总时间一般是固定的，称为周期(注:周期的倒数是频率)。高电平输出的时间通常称为脉宽，占空比是脉宽(PW)与波形总周期(T)之比的百分比。高电平输出持续时间越长，占空比越长，模拟信号中相应的电压也就越高。下图显示了对应于脉冲宽度0%-100%的模拟信号电压在0V-3.3V(高电平为3.3V)之间的变化情况.

![](media/a439e1bd8a4578b43b7188c821d58594.jpeg)

PWM占空比越长，输出功率越高。既然我们了解了这种关系，我们就可以用PWM来控制LED的亮度或直流电机的速度等等。从上面可以看出，PWM并不是真实的模拟信号，电压的有效值等于相应的模拟信号。因此，我们可以控制LED和其他输出模块的输出功率，以达到不同的效果

树莓派Pico与 PWM

树莓派Pico板有16个PWM通道，每个PWM通道可以独立控制频率和占空比，时钟频率范围为7Hz到125MHz。树莓派Pico板上的每个引脚都可以配置为PWM输出。

4.项目电路图和接线图：

![](media/cb069d7553d861e3293d8bdbe85bbd05.png)

![](media/96800765a20d72653a8cd4a9ae12b636.png)

5.项目代码：

本项目设计使GP16输出PWM，脉宽由0%逐渐增加到100%，再由100%逐渐减小到0%。

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
04：呼吸灯”。并鼠标左键双击“Project_04_Breathing_Led.py”。

![](media/2b0448e680fd674386890d00214e9574.png)

6.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/4b9addaabd59a3dcad229ab07318e956.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：电路中的LED从暗逐渐变亮，再从亮逐渐变暗，就像呼吸一样。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/22261aaf04bc71e3d2bab4f220c3672a.png)

![](media/e4789bf063f7fdca158b7a87011a02de.png)
![](media/3673c95868f245ee28365de8e51d2ced.png)

### 项目 05：交通灯

1.项目介绍：

交通灯在我们的日常生活中很普遍。根据一定的时间规律，交通灯是由红、黄、绿三种颜色组成的。每个人都应该遵守交通规则，这可以避免许多交通事故。在这个项目中，我们将使用树莓派Pico板和一些led(红，黄，绿)来模拟交通灯。

2.项目元件：

|![](media/e9de1e032b926d52712bfc484e6cdfe7.jpeg)|![](media/03091fc80bb79b974846932ee4dfeb49.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/afa6edd3ff90b027a6f43995a6fb15a2.png)|![](media/0c1b0f91b4e56bcbc235d06b48809ac9.png)|
|-|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|公对母杜邦线若干|红色LED*1|黄色 LED*1|
|![](media/6c688493b558ed5f3e90e7dab38cbd93.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/b57b4057770f0bcc43f037c0ab8e1c41.png)|![](media/c801a7baee258ff7f5f28ac6e9a7097b.png)|
|绿色LED*1|USB 线*1|220Ω电阻*3|面包板*1|跳线若干|

3.项目电路图和接线图：

![](media/92bcb9557428316b25d5273e25665210.png)![](media/41ae8ac64c0c776dd22e6518240c56a1.png)

4.项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2.
项目课程”→“项目05：交通灯”。并鼠标左键双击“Project_05_Traffic_Lights.py”。

![](media/f413bef844529ec9d7a7a68d707b82e7.png)

5.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/2f5fecc1873220df106fec5692ff52fb.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：1.首先，绿灯会亮5秒，然后熄灭；2.其次，黄灯会闪烁3次，然后熄灭；3.然后，红灯会亮5秒，然后熄灭；4.继续运行上述1-3个步骤。

按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/ca10dd2d2ada63dff4e6b9ef07198644.png)

### 项目 06: RGB LED

1.项目介绍：

![](media/94bdff69e438989d8e0934e57f2e5c00.png)

RGB led由三种颜色(红、绿、蓝)组成，通过混合这三种基本颜色可以发出不同的颜色。在这个项目中，我们将向你介绍RGB LED，并向你展示如何使用树莓派Pico板控制RGB LED发出不同的颜色光。即使RGB LED是非常基本的，但这也是一个介绍自己或他人电子和编码基础的伟大方式。

2.项目元件：

|![](media/b18fe281156b29c44796f72222718d58.jpeg)|![](media/03091fc80bb79b974846932ee4dfeb49.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/f1a86fc81ab4b043263ce7e01e14d470.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|公对母杜邦线若干|RGB LED*1|
|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)||
|220Ω电阻*3|面包板*1|USB 线*1||

3. 元件知识：

显示器大多遵循RGB颜色标准，电脑屏幕上的所有颜色都是由红、绿、蓝三种颜色以不同比例混合而成。

![](media/32abd117bdfbba2f79a0e156048b9d22.png)![](media/5a0792145e8a7d9038bf9de389d75fc6.png)

这个RGB LED有4个引脚，每个颜色(红，绿，蓝)和一个共同的阴极。为了改变RGB led的亮度，我们可以使用树莓派Pico板的PWM引脚。PWM引脚会给RGB led不同占空比的信号以获得不同的颜色。

如果我们使用3个10位PWM来控制RGBLED，理论上我们可以通过不同的组合创建210\*210\*210=
1,073,741,824(10亿)种颜色。

4.  项目电路图和接线图：

![](media/f6950bc8498e6139cbb67db84cdd5a9a.png)

![](media/c18f869a9b18fc521c3d09be942efebd.png)

注意：

RGB LED最长引脚(共阴极)连接GND。

![](media/1584356c63bf99934ae0810ee02dced3.png)

怎样识别五色环220Ω电阻

![](media/793740d0b936e516ca354111e2d0eb79.png)

5.项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2.
项目课程”→“项目06：RGB”。并鼠标左键双击“Project_06_RGB_LED.py”。

![](media/e657fa73d15780eee2232e38bd417384.png)

6.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/25b3986effb8cafefcaaff98553b19dc.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：RGB LED开始显示随机颜色。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/9a98915a2eb9285bd0b171968795a85d.png)

### 项目 07: 流水灯

1.项目介绍：

在日常生活中，我们可以看到许多由不同颜色的led组成的广告牌。他们不断地改变灯光(像流水一样)来吸引顾客的注意。在这个项目中，我们将使用树莓派Pico板控制10个leds实现流水的效果。

2.项目元件：

|![](media/b18fe281156b29c44796f72222718d58.jpeg)|![](media/68aa11662f0455d6b5f1965a29336313.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/3ec5906fad2172708d449390140f55e6.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|公对母杜邦线若干|红色LED*10|
|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/c801a7baee258ff7f5f28ac6e9a7097b.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|220Ω电阻*10|面包板*1|跳线若干|USB 线*1|

3.项目电路图和接线图:

![](media/e6f92039d131685369db2d1ac2c30267.png)

![](media/e3d6a1880f61fdfaec74360190f5ed43.png)

注意:

怎样连接LED

![](media/14a84d5f016d7566151a5563c502787e.png)

怎样识别五色环220Ω电阻

![](media/793740d0b936e516ca354111e2d0eb79.png)

4.项目代码：

本项目是设计制作一个流水灯。这是这些行动：首先打开LED
\#1，然后关闭它。然后打开LED
\#2，然后关闭…并对所有10个LED重复同样的操作，直到最后一个LED关闭。这一过程反复进行，以实现流水的“运动”。

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
07：流水灯”。并鼠标左键双击“Project_07_Flowing_Water_Light.py”。

![](media/0eb44c3d63b1a75b725752fab046d8de.png)

5.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/5e5bd0305862a931c369da405aad1cd0.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：10个LED将从左到右点亮，然后从右到左返回。按“Ctrl+C”或点单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/56af2327f55a5b9499db9634d474fe65.png)

![](media/912e2c3f88b522b89b9935548bae3bd9.png)

### 项目 08: 一位数码管

1. 项目介绍：

七段数码管是一种显示十进制数字的电子显示设备，广泛应用于数字时钟、电子仪表、基本计算器和其他显示数字信息的电子设备。甚至我们在电影中看到的炸弹也有七段数码管。也许七段数码管看起来不够现代，但它们是更复杂的点阵显示器的替代品，在有限的光线条件下和强烈的阳光下都很容易使用。在这个项目中，我们将使用树莓派Pico板控制一位数码管显示数字。

2.  项目元件：

|![](media/b18fe281156b29c44796f72222718d58.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/75e38d601750a4707369bc73d8028063.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|公对母杜邦线若干|一位数码管*1|
|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)||
|220Ω电阻*8|面包板*1|USB 线*1||

3. 元件知识：

![](media/f63a087723b81874721e0c133a078c75.png)

一位数码管显示原理：数码管显示是一种半导体发光器件。它的基本单元是一个发光二极管(LED)。数码管显示根据段数可分为7段数码管和8段数码管。8段数码管比7段多一个LED单元(用于小数点显示)。七段LED显示屏的每段是一个单独的LED。根据LED单元接线方式，数码管可分为共阳极数码管和共阴极书案管。

在共阴极7段数码管中，分段LED的所有阴极(或负极)都连接在一起，你应该把共阴极连接到GND，要点亮一个分段LED，你可以将其关联的引脚设置为HIGH。

在共阳极7段数码管中，所有段的LED阳极(正极)都连接在一起，你应该把共阳极连接到+5V。要点亮一个分段LED，你可以将其关联的引脚设置为LOW。

![](media/570d533e2307bf68aee145d544ab5939.png)

数码管的每个部分由一个LED组成。所以当你使用它的时候，你也需要使用一个限流电阻。否则，LED会被烧坏。在这个实验中，我们使用了一个普通的共阴极一位数码管。正如我们上面提到的，你应该将公共阴极连接到GND。要点亮一个分段LED，你可以将其关联的引脚设置为HIGH。

4.项目电路图和接线图：

![](media/cdecc109f3d703edb67b372d8c05a696.png)

注意：插入面包板的七段数码管方向与接线图一致，右下角多一个点。

![](media/4429ccfb9623a9a3975cdf217c927204.png)

![](media/1aea8db87a3e0929caecb82b4b4690dc.png)

5.项目代码：

数字显示分7段，小数点显示分1段。当显示某些数字时，相应的段将被点亮。例如，当显示数字1时，b和c段将被打开。

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
08：一位数码管”。并鼠标左键双击“Project_08_One_Digit_Digital_Tube.py”。

![](media/a3d95d475b610c47edd8ecb5a5b1a171.png)

6.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/fdcccee3c5534c97757ef0546fced860.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：一位数码管将显示从9到0的数字。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/9fb1bc3b2e6a4d7e7ee085ef5296a87c.png)

### 项目 09：四位数码管

1.  项目介绍：

四位数码管是一种非常实用的显示器件，电子时钟的显示，球场上的记分员，公园里的人数都是需要的。由于价格低廉，使用方便，越来越多的项目将使用4位数码管。在这个项目中，我们使用树莓派Pico板控制四位数码管来显示数字。

2.  项目元件：

|![](media/3494ab155507e129f563102efb9faebb.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/ee7a4ecd35ef268149e31fb9d62c8227.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|220Ω 电阻*8|四位数码管*1|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)||
|面包板*1|公对母杜邦线若干|USB 线*1||

3.  元件知识：

![](media/ce987bf9a2ab398945c98b34d3f8a003.png)

四位数码管：四位数码管有共阳极和共阴极两种四位数码管，显示原理是和一位数码管是类似的，都是8个GPIO口控制数码管的显示段，就是8个led灯，不过，这里是4位的，所以就还需要4个GPIO口来控制位选择端，就是选择哪个单个数码管亮，位的切换很快，肉眼区分不出来，就能看起来是多个数码管同时显示的了。

我们的四位数码管是共阴极的。

下图为4位数码管的引脚图，G1、G2、G3、G4就是控制位的引脚。

![](media/37113fa53213973132086c285d67686b.png)

下图为4位数码管内部布线原理图

![](media/c210e9899274cdf79ffd44db1e250fb5.png)![](media/ea75d1b7414bf6f8c187fb32fea9bc83.png)

4.项目电路图和接线图：

![](media/4f64b9bf6b74ab49584f69c7465efa73.png)

![](media/c4bb871135269a61e7341e7a5360b70d.png)

5.项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
09：四位数码管”。然后鼠标左键双击“Project_09_Four_Digit_Digital_Tube.py”。

![](media/ec2b6701848dadab7ee84f486dc51429.png)

6.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/7c583ae0a148563180a43e1a3e8cf9a3.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：四位数码管显示数字，并在一个无限循环中重复这些动作。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/5abe40d65ab6101d7b6aee654810fb56.png)

### 项目 10：8×8 点阵显示

1.  项目介绍：

点阵屏是一种电子数字显示设备，可以显示机器、钟表、公共交通离场指示器和许多其他设备上的信息。在这个项目中，我们将使用树莓派Pico板控制8x8 LED点阵来逐渐点亮点阵。

2.  项目元件：

|![](media/b18fe281156b29c44796f72222718d58.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/d226a1f3c801ac78321f0692143c853e.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|8*8点阵屏*1|USB 线*1|
|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)||
|公对母杜邦线若干|220Ω 电阻*8|面包板*1||

3.  元件知识：

8\*8LED Matrix：8\*8点阵，就是由64个led灯组成，有行共阳极和行共阴极两种，我们的模块是行共阳极的，也就是每一行有一条线将LED的正极连到一起，列就是将LED灯的负极连接到一起，看下图：

![](media/69c719a7898907ab32f089f0cbbaff13.png)

![](media/bcfa2498367eaf9c7733da15af32eae7.png)

4.  项目电路图和接线图：

![](media/dc2d64f3098b039937483e04589cbc17.png)

![](media/3b050fbaf0be0037f5cc2a215d544306.png)

5.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目 10：8×8
点阵显示”。然后鼠标左键双击“Project_10_8×8_Dot_Matrix_Display.py”。

![](media/e2089a7259c8c656e7d9f20cc082e6f5.png)

6.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/e59e1ea4d7917de01bd09629920d2cbd.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：8\*8点阵屏显示字符“A”1S、显示字符“B”1S、显示字符“C”1S，然后滚屏显示字符串“Hello World”，反复循环。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/e9e4bc9d5bcac5f8b11d8224a906a8e4.png)

### 项目 11：74HC595N 控制 8 个LED

1.项目介绍：

在之前的项目中，我们已经学过了怎样点亮一个LED。

树莓派Pico板上只有26个IO端口，我们如何点亮大量的led呢?
有时可能会耗尽树莓派Pico板上的所有引脚，这时候就需要用移位寄存器扩展它。你可以使用74HC595N芯片一次控制8个输出，而只占用你的微控制器上的几个引脚。你还可以将多个寄存器连接在一起，以进一步扩展输出，在这个项目中，我们将使用树莓派Pico板，74HC595芯片和LED制作一个流水灯来了解74HC595芯片的功能。

2.项目元件：

|![](media/b18fe281156b29c44796f72222718d58.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/f97e58ab51ec0a274ff3e72e08a7d55d.png)|
|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|74HC595N芯片*1|
|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/c801a7baee258ff7f5f28ac6e9a7097b.png)|
|220Ω电阻*8|面包板*1|跳线若干|
|![](media/3ec5906fad2172708d449390140f55e6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|
|红色LED*8|USB 线*1|公对母杜邦线若干|

3.  元件知识：

![](media/6921c6d60135e072ed4bd24564ec4a6d.png)

74HC595N芯片：简单来说就是具有8
位移位寄存器和一个存储器，以及三态输出功能。移位寄存器和存储器同步于不同的时钟，数据在移位寄存器时钟SCK的上升沿输入，在存储寄存器时钟RCK的上升沿进入的存储寄存器中去。如果两个时钟连在一起，则移位寄存器总是比存储寄存器早一个脉冲。移位寄存器有一个串行移位输入端（SI）和一个用于级联的串行输出端（SQH）,8位移位寄存器可以异步复位（低电平复位），存储寄存器有一个8位三态并行的总线输出，当输出使能（OE）被使能（低电平有效）将存储寄存器中输出至74HC595N的引脚（总线）。

![](media/858b189f06ad68afe051b15043b2affd.png)

引脚说明：

|13引脚OE|是一个输出使能引脚，用于确保锁存器的数据是否输入到Q0-Q7引脚。在低电平时，不输出高电平。在本实验中，我们直接连接GND，保持低电平输出数据。|
|-|-|
|14引脚SI|这是74HC595接收数据的引脚，即串行数据输入端，一次只能输入一位，那么连续输入8次，就可以组成一个字节了。|
|10引脚SCLR|一个初始化存储寄存器管脚的管脚。在低电平时初始化内部存储寄存器。在这个实验中，我们连接VCC以保持高水平。|
|11引脚SCK|移位寄存器的时钟引脚，上升沿时，移位寄存器中的数据整体后移，并接收新的数据输入|
|12引脚RCK|存储寄存器的时钟输入引脚。上升沿时，数据从移位寄存器转存到存储寄存器中。这时数据就从Q0~Q7端口并行输出。|
|9引脚SQH|引脚是一个串行输出引脚，专门用于芯片级联，接下一个74HC595的SI端|
|Q0--Q7(15引脚，1-7引脚)|八位并行输出端，可以直接控制数码管的8个段|

4.  项目电路图和接线图：

![](media/1738cecf584c83b55370153ebc1688b7.png)

注意：需要注意74HC595N芯片插入的方向

![](media/ec1ecffbdf054501b67abeeb96917e73.png)
![](media/5a0de137092d094f6007098ac141586a.png)

![](media/c96c92db4125b2cc518a0ed5f72e33f9.png)

5.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目 11：74HC595N
控制 8 个LED”。选择“my74HC595.py”，鼠标右键单击选择
“上载到/”，等待“my74HC595.py”被上传到Raspberry Pi Pico，然后鼠标左键双击“Project_11_74HC595N_Controls_8_LEDs.py”。

![](media/0b21ec2c89409d86bdec8909a9bb0344.png)

![](media/297892c987e3ff99c5e4289ad3046379.png)

6.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/7da0606b255f4327a485b5713f5f54f4.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：8个LED开始以流水模式闪烁。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/e9d7cdf21bcce16161922be2a0f02137.png)

### 项目 12：有源蜂鸣器

1.项目介绍：

有源蜂鸣器是一个发声组件。它被广泛用作电脑、打印机、报警器、电子玩具、电话、计时器等的发声元件。它有一个内在的振动源，只需连接5V电源，即可持续发出嗡嗡声。在这个项目中，我们将使用树莓派Pico板控制有源蜂鸣器发出“滴滴”声。

2.  项目元件：

|![](media/2db038cb38e0beabf2f9e14043d23a6f.jpeg)|![](media/f39510c60d4c43dfca4e26b0bdb9aae7.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)|
|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|面包板*1|
|![](media/9197d4aff9356c585b7ef68e33a6881d.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/c801a7baee258ff7f5f28ac6e9a7097b.png)|
|NPN型晶体管(S8050)*1|1kΩ电阻*1|跳线若干|
|![](media/4b4f653a76a82a3b413855493cc58fba.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|
|有源蜂鸣器*1|USB 线*1|公对母杜邦线若干|

3. 元件知识：

![](media/11ec5ddc982db9928341e858aab94652.png)

有源蜂鸣器内部有一个简单的振荡器电路，可以将恒定的直流电转换成特定频率的脉冲信号。一旦有源蜂鸣器收到一个高电平，它将产生声音。而无源蜂鸣器是一种内部没有振动源的集成电子蜂鸣器，它必须由2K-5K方波驱动，而不是直流信号。这两个蜂鸣器的外观非常相似，但是一个带有绿色电路板的蜂鸣器是无源蜂鸣器，而另一个带有黑色胶带的是有源蜂鸣器。无源蜂鸣器不能区分正极性而有源极性蜂鸣器是可以。如下所示：

![](media/76d53f3b35afaa98712e855302e44e32.png)

![](media/9197d4aff9356c585b7ef68e33a6881d.png)

晶体管:
由于蜂鸣器需要很大的电流，ESP32输出能力的GPIO不能满足要求，这里需要一个NPN型晶体管来放大电流。晶体管，全称:半导体晶体管，是一种控制电流的半导体器件。晶体管可以用来放大微弱信号，也可以用作开关。它有三个电极(pin)：基极(b)，集电极(c)和发射极(e)。当电流通过“be”之间时，“ce”将允许几倍的电流通过(晶体管放大)，此时，晶体管在放大区工作。当“be”之间的电流超过某个值时，“ce”将不再允许电流增加，此时晶体管工作在饱和区。晶体管有两种类型如下所示：PNP和NPN

![](media/02dad9f2fcac0d7bfe4cc135d2301aa6.png)

PNP晶体管 NPN晶体管

在我们的套件中，PNP晶体管标记为8550,NPN晶体管标记为8050。

基于晶体管的特性，它常被用作数字电路中的开关。由于单片机输出电流的能力很弱，我们将使用晶体管来放大电流和驱动大电流的元件。在使用NPN晶体管驱动蜂鸣器时，通常采用以下方法：如果GPIO输出高电平，电流将流过R1，晶体管将传导，蜂鸣器将发出声音。如果GPIO输出低电平，没有电流流过R1，晶体管就不会传导，蜂鸣器也不会响。在使用PNP晶体管驱动蜂鸣器时，通常采用以下方法：如果GPIO输出低电平，电流将流过R1，晶体管将传导，蜂鸣器将发出声音。如果GPIO输出高电平，没有电流流过R1，晶体管就不会传导，蜂鸣器也不会响。

![](media/e33aa5534aa1bd11e4ca2fa51c5b6548.png)

4.  项目电路图和接线图：

![](media/8b84654a0f04d7e4c5f9c2f2923e577b.png)

![](media/6e607b53416c90c3573d3f890f8a5ed0.png)

注意：1.该电路中蜂鸣器的电源为5V。在3.3V的电源下，蜂鸣器可以工作，但会降低响度。

2.VUSB应连接到USB线的正极，如果它连接到GND，它可能烧坏电脑或树莓派Pico板。同样，树莓派Pico板的36-40引脚接线时也要小心，避免短路。

3.有源蜂鸣器正极(“+”/长引脚)接引脚16，负极（短引脚）接GND。

5.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
12：有源蜂鸣器”。并鼠标左键双击“Project_12_Active_Buzzer.py”。

![](media/f183ff22904cd00ff0237cae08b9540f.png)

6.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/c75586103b8592a5d7fa414ca8518343.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：有源蜂鸣器发出“滴滴”声。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/18db0b896bb5978a88a2c4f053c1d0ae.png)

### 项目 13：无源蜂鸣器

1.项目介绍：

在之前的项目中，我们研究了有源蜂鸣器，它只能发出一种声音，可能会让你觉得很单调。这个项目将学习另一种蜂鸣器，无源蜂鸣器。与有源蜂鸣器不同，无源蜂鸣器可以发出不同频率的声音。在这个项目中，你将使用树莓派Pico板控制无源蜂鸣器发出警报声。

2.  项目元件：

|![](media/e796f897747c8b2786364a0a1b18fe07.jpeg)|![](media/48434ce34b111ef48f78bd7f777dbcfd.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)|
|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|面包板*1|
|![](media/9197d4aff9356c585b7ef68e33a6881d.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/aa06e883415a425c727a539a8267ac7a.png)|
|NPN型晶体管(S8050)*1|1kΩ电阻*1|跳线若干|
|![](media/d1ea1bb2b2749820cab389d5b85b838b.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|
|无源蜂鸣器*1|USB 线*1|公对母杜邦线若干|

3.  元件知识：

![](media/1599686e26b4ccea33669334f93b956a.png)

无源蜂鸣器是一种内部没有振动源的集成电子蜂鸣器。它必须由2K-5K方波驱动，而不是直流信号。这两个蜂鸣器的外观非常相似，但是一个带有绿色电路板的蜂鸣器是无源蜂鸣器，而另一个带有黑色胶带的是有源蜂鸣器。无源蜂鸣器不能区分正极性而有源极性蜂鸣器是可以。

![](media/fc42c5ed014609ff0b290ee5361bb2fd.png)

晶体管: 请参考项目12.

4.项目电路图和接线图:

![](media/88e1667cdd09ffa9394f7aae9ce60242.png)

![](media/0257f2526dcedd215a11ccbce45ded51.png)

5.项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.项目课程”中。你可以把代码移到任何地方。例如，我们将“2.项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
13：无源蜂鸣器”。并鼠标左键双击“Project_13_Passive_Buzzer.py”。

![](media/0a66fe50bcfb6a1e72af093da1cb0dfc.png)

6.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/b43f44493a495bb9b505d4308b2de076.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：无源蜂鸣器发出警报声。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/fcc13d87fb1f336d65bf0149791aed85.png)

### 项目 14: 小台灯

1.项目介绍：

你知道树莓派Pico可以在你按下按键的时候点亮LED吗?
在这个项目中，我们将使用树莓派Pico板，一个按键开关和一个LED来制作一个迷你台灯。

2.项目代码：

|![](media/d7bde912c31f86d5e3854e608a5ff08f.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/5b8fea4657b47510d199f740fdcaaa9d.png)|![](media/ef77f5a64c382157fc2dea21ec373fef.png)|![](media/da8a2a9d15baf7280966f3fdbb025a8c.png)|
|-|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|按键*1|红色 LED*1|10KΩ电阻*1|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/845d05a6108b1662b828610ba9dcb788.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|![](media/b006569d007392f7ebcd1a2d84c0c942.png)|![](media/9cab81f7da18c7b0c245ec2a2f614f3a.png)|
|面包板*1|220Ω电阻*1|USB 线*1|公对母杜邦线若干|按键帽*1|

3.元件知识：

![](media/5b8fea4657b47510d199f740fdcaaa9d.png)

按键：按键可以控制电路的通断，把按键接入电路中，不按下按键的时候电路是断开的，

一按下按键电路就通啦，但是松开之后就又断了。可是为什么按下才通电呢？这得从按键的内部构造说起。没按下之前，电流从按键的一端过不去另一端；按下的时候，按键内部的金属片把两边连接起来让电流通过。

按键内部结构如图：![](media/d2a204e61c768f18924150db58aee093.png)，未按下按键之前，1、2就是导通的，3、4也是导通的，但是1、3或1、4或2、3或2、4是断开（不通）的；只有按下按键时，1、3或1、4或2、3或2、4才是导通的。

在设计电路时，按键开关是最常用的一种元件。

按键的原理图:     
![](media/5e42fde9876f9be810d85a7fb8b331f7.png)
![](media/8677548f9e756281629430d66ba3a460.png)  
什么是按键抖动？

我们想象的开关电路是“按下按键-立刻导通”“再次按下-立刻断开”，而实际上并非如此。

按键通常采用机械弹性开关，而机械弹性开关在机械触点断开闭合的瞬间（通常
10ms左右），会由于弹性作用产生一系列的抖动，造成按键开关在闭合时不会立刻稳定的接通电路，在断开时也不会瞬时彻底断开。

![](media/4dbcca62c2d75cab03260584924a16d8.jpeg)

那又如何消除按键抖动呢？

常用除抖动方法有两种：软件方法和硬件方法。这里重点讲讲方便简单的软件方法。

我们已经知道弹性惯性产生的抖动时间为10ms
左右，用延时命令推迟命令执行的时间就可以达到除抖动的效果。

所以我们在代码中加入了0.02秒的延时以实现按键防抖的功能。

![](media/1497573e05f993b5f32923fcd6590a01.jpeg)

4. 项目电路图和接线图：

![](media/19f9dcfaacc32a6bc8ae16e362aa3122.png)

![](media/1c75a05a53faacfca9592631619909b0.png)

注意:

怎样连接LED

![](media/14a84d5f016d7566151a5563c502787e.png)

怎样识别五色环220Ω电阻和五色环10KΩ电阻

![](media/793740d0b936e516ca354111e2d0eb79.png)

![](media/18484e5d16b6d89c63825cc2efa6a543.png)

5.项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
14：小台灯”。并鼠标左键双击“Project_14_Mini_Table_Lamp.py”。

![](media/3dffca1a60f2c48c75252d77e1f361c5.png)

6.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/e949fe64374ed67a33a7d84048b930a9.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：按下按钮，LED亮起；当按钮松开时，LED仍亮着。再次按下按钮，LED熄灭；当按钮释放时，LED保持关闭。是不是很像个小台灯？按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/09cd933d68282c274875dea655212fea.png)

### 项目 15：模拟沙漏

1.  项目介绍：

古代人没有电子时钟，就发明了沙漏来测时间，沙漏两边的容量比较大，在一边装了细沙，中间有个很小的通道，将沙漏直立，有细沙的一边在上方，由于重力的作用，细沙就会往下流通过通道到沙漏的另一边，当细沙都流到下边了，就倒过来，把一天反复的次数记录下来，第二天就可以通过沙漏反复流动的次数而知道这一天大概的时间了。这一课我们将利用树莓派Pico板控制倾斜开关和LED灯来模拟沙漏，制作一个电子沙漏。

2.  项目元件：

|![](media/222aee34a428755aaf97b711ded3f09a.jpeg)|![](media/03091fc80bb79b974846932ee4dfeb49.png)|![](media/36f15610f430e5d5138f4e4fb721c40f.png)|![](media/ef77f5a64c382157fc2dea21ec373fef.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|倾斜开关*1|红色 LED*4|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/845d05a6108b1662b828610ba9dcb788.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)||
|面包板*1|220Ω电阻*4|USB 线*1||
|![](media/da8a2a9d15baf7280966f3fdbb025a8c.png)|![](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)||
|10KΩ电阻*1|跳线若干|公对母杜邦线若干||

3.元件知识：

![](media/8c40739f8e05f753f145420b421a0f47.png)

倾斜开关也叫数字开关。里面有一个可以滚动的金属球。采用金属球滚动与底部导电板接触的原理来控制电路的通断。当倾斜开关是滚珠型倾斜感应单方向性触发开关，当倾斜传感器向触发端（两根金属脚端）倾斜时，倾斜开关处于闭路状态，模拟端口的电压约为5V(二进制数为1023)。这样，LED会亮起。当倾斜开关在水平位置或向另一端倾斜时，倾斜开关处于开路状态，模拟端口的电压约为0V(0二进制)。LED将会关闭。在程序中，我们根据模拟端口的电压值，是否大于2.5V(512二进制)来判断开关是开还是关。

这里用倾斜开关的内部结构来说明它是如何工作的，显示如下图：

![](media/40bc569b295c4656bd973da4ad8734e2.png)

4.项目电路图和接线图：

![](media/033b2d8368f73658fff3b00d8508e4f3.png)

![](media/157dda6c8dad94ceddcb2cea06f69f03.png)

注意: 怎样连接LED

![](media/14a84d5f016d7566151a5563c502787e.png)

怎样识别五色环220Ω电阻和五色环10KΩ电阻

![](media/793740d0b936e516ca354111e2d0eb79.png)

![](media/18484e5d16b6d89c63825cc2efa6a543.png)

5.项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
15：模拟沙漏”。并鼠标左键双击“Project_15_Tilt_And_LED.py”。

![](media/8e7b27e0e8565b5c09643ff3bd01e151.png)

6.项目结果：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/7644c375cceed19c406e8b4573dbdb62.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：将面包板倾斜到一定角度，led就会一个一个地亮起来。当回到上一个角度时，led会一个一个关闭。就像沙漏一样，随着时间的推移，沙子漏了出来。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/b938dec40f1377e27eb88bc299315a09.png)

### 项目 16：防窃警报器

1.  项目介绍：

人体红外传感器测量运动物体发出的热的红外(IR)线。该传感器可以检测人、动物和汽车的运动，从而触发安全警报和照明。它们被用来检测移动，是安全的理想选择，如防盗警报和安全照明系统。在这个项目中，我们将使用树莓派Pico板控制人体红外传感器、蜂鸣器和LED来模拟防盗报警器。

2.  项目元件：

|![](media/070789ba62f5044f894eb126635a43e5.jpeg)|![](media/03091fc80bb79b974846932ee4dfeb49.png)|![](media/239131563f68fbf379e97d8384cf2d9b.png)|![](media/4b4f653a76a82a3b413855493cc58fba.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|人体红外传感器*1|有源蜂鸣器*1|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/845d05a6108b1662b828610ba9dcb788.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|面包板*1|公对母杜邦线若干|220Ω电阻*1|USB 线*1|
|![](media/ef77f5a64c382157fc2dea21ec373fef.png)|![](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/9197d4aff9356c585b7ef68e33a6881d.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|
|红色 LED*1|跳线若干|NPN型晶体管(S8050)*1|1kΩ电阻*1|
|![](media/ebfacf0e05bcd3941fe3b641935756b0.png)||||
|3Pin 杜邦母单*1||||

3.  元件知识：

人体红外传感器：其原理是某些晶体，例如钽酸锂、硫酸三甘肽等受热时，晶体两端会产生数量相等、符号相反的电荷，将这些电荷经放大器可转换为电压输出。而人体是会释放红外线的，虽然比较微弱，但是还是可以检测得到的。人体红外传感器检测附近有人运动时，传感器信号端输出高电平1，否则输出低电平0。特别注意，这个传感器可以检测在运动中的人、动物和汽车，静止中的人、动物和汽车是检测不到的，检测最远距离大约为7米左右。

注意：人体红外传感器应避开日光、汽车头灯、白炽灯直接照射，也不能对着热源(如暖气片、加热器)或空调，以避免环境温度较大的变化而造成误报。同时还易受射频辐射的干扰。

传感器技术参数：

最大输入电压：DC 3.3 ~ 5 v

最大工作电流：50MA

最大功率：0.3W

工作温度：-20 ~ 85℃

输出高电平3V，低电平0 V

延迟时间：大约2.3到3秒钟

检测角度：大约100度

检测最远距离：大约 7米左右

指示灯输出(当输出高电平时，它将点亮)

引脚限制电流：50MA

传感器原理图：

![](media/9e1ec604aa6f9d4a3c1fe41d4bccd699.png)

4.  项目电路图和接线图：

![](media/694b0402398d04cd0a42f449dcdd0f61.png)

![](media/a9539236b5a3cfbce85a0b67691083e2.png)

5.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
16：防窃警报器”。并鼠标左键双击“Project_16_Burglar_Alarm.py”。

![](media/4995a7eca564050b86c07eb82ac2e7f7.png)

6.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/b1894b924fca537ba37bc25116a281e8.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：如果人体红外传感器检测到附近有人移动时，蜂鸣器就会不断地发出警报，且LED不断地闪烁，同时Thonny IDE下的”Shell”窗口将打印字符串"ALARM! Motion detected!"。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/50957b131c06be90f2641331f6476f17.png)

### 项目 17： I2C 128×32 LCD

1.项目介绍：

在生活中，我们可以利用显示器等模块来做各种实验。你也可以DIY各种各样的小物件。例如，用一个温度传感器和显示器做一个温度测试仪，或者用一个超声波模块和显示器做一个距离测试仪。下面，我们将使用LCD_128X32_DOT模块作为显示器，将其连接到树莓派Pico板上。将使用树莓派Pico板控制LCD_128X32_DOT显示屏显示各种英文文字、常用符号和数字。

2.项目元件： 

|![](media/b1265f71184b5d144248ea3e847a18c9.jpeg)|![](media/770714fabf173efb3ef34d9f84d09798.png)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|
|-|-|-|
|树莓派Pico板*1|LCD_128X32_DOT*1|树莓派Pico板的扩展板*1|
|![](media/e615c2849ce15bdfc8e26432004124ec.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)||
|4P 转杜邦线母单10厘米*1|USB 线*1||

3.元件知识：

![](media/770714fabf173efb3ef34d9f84d09798.png)

LCD_128X32_DOT：一个像素为128\*32的液晶屏模块，它的驱动芯片为ST7567A。模块使用IIC通信方式，同时，代码中包含所有英文字母和常用符号的库，可以直接调用。使用时，我们还可以在代码中设置，让英文字母和符号显示不同文字大小。为了方便设置图案显示，我们还提供一个取模软件，可将特定的图案转化成控制代码，然后直接复制到测试代码中使用的。

LCD_128X32_DOT原理图：

![](media/5451aed32bc5b7b30fbd5613ad09a65b.png)

LCD_128X32_DOT技术参数：

显示像素：128\*32 字符

芯片工作电压：4.5 ~ 5.5V

工作电流：100mA (5.0V)

模块最佳工作电压：5.0V

4.  项目接线图：

特别注意：这里必须使用4P     转杜邦线母单10厘米连接LCD_128X32_DOT，LCD_128X32_DOT才会显示正常；否则，使用4P     转杜邦线母单20厘米，LCD_128X32_DOT可能会显示不正常。

![](media/37c015266b4998c76a04be21f0d0a969.png)

5.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目 17： I2C 128×32 LCD”。分别选择“lcd128_32.py”和 “lcd128_32_fonts.py”，右键单击鼠标选择
“上载到/”，等待“lcd128_32.py”和 “lcd128_32_fonts.py”被上传到Raspberry Pi Pico，并鼠标左键双击“Project_17_I2C_128_32_LCD.py”。

![](media/236c8b87b83b277c44fe439e7d48a201.png)

![](media/0600c92c1815ce24c5881433f94be3f9.png)

![](media/ca315bba68e8f923b69f6fb261d04bad.png)

6.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/f6c52c74beb5ddbc587dad2d620b7b83.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：128X32LCD模块显示屏第一行显示“keyes”、第二行显示“ABCDEFGHIJKLMNOPQR”、第三行显示“123456789+-\*/\<\>=$@”、第四行显示“%^&(){}:;'|?,.~\\\[\]”。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/6bffa4c9e8d34b4487d1212e464e8897.png)

### 项目 18：小风扇

1.  项目介绍：

在炎热的夏季，需要电扇来给我们降温，那么在这个项目中，我们将使用树莓派Pico板控制直流电机模块和小扇叶来制作一个小电扇。

2.  项目元件：

|![](media/3bd15bd23899295db77b3fde23d6f227.jpeg)|![](media/a148c40620767714cde78f41a4822528.png)|![](media/df3db6765ee8c86beafa8410e87dd50d.png)|
|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|跳线若干|
|![](media/5fe5f8cd6e75e7f8d4ec71f54a4ac2f5.png)|![](media/4e0b78edf6e4aeefa4c5191c606b2031.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|L293D芯片*1|面包板*1|USB 线*1|
|![](media/5eba8bae9e1d18b959ca425a9cc83fd2.jpeg)|![](media/655e6c465cb423279e0908513a983711.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|
|直流电机*1|风扇片*1|公对母杜邦线若干|

3.元件知识:

![](media/5fe5f8cd6e75e7f8d4ec71f54a4ac2f5.png)

L293D芯片：L293D是一种直流电动驱动IC，在一些机器人项目中可用来驱动直流电机或步进电机。它共有16个引脚，可以同时驱动两路直流电机。输入电压范围：4.5 V ~ 36 V，每通道输出电流：MAX 600mA，可以驱动感性负载，特别是其输入端可以与单片机直接相连，从而很方便地受单片机控制。当驱动小型直流电机时，可以直接控制两路电机，并且可以实现电机正转与反转，实现此功能只需改变输入端的高低电平。市面上有许多采用L293D芯片的电机驱动板，当然我们也可以自己通过简单连接来使用它。

L293D引脚图：

![](media/2e5e0bd5b4577ac159d0568404dc21b5.png)

|引脚号|引脚名称|描述|
|-|-|-|
|1|Enable1|该引脚使能输入引脚Input 1(2)和Input 2(7)|
|2|In1|直接控制输出1引脚，由数字电路控制。|
|3|Out1|连接到电机1的一端|
|4|0V|接地引脚连接到电路的接地(0V)|
|5|0V|接地引脚连接到电路的接地(0V)|
|6|Out2|连接到电机1的另一端|
|7|In2|直接控制输出2引脚。由数字电路控制|
|8|+V motor|连接到运行电机的电压引脚(4.5V至36V)|
|9|Enable2|该引脚使能输入引脚输入3(10)和输入4(15)|
|10|In3|直接控制输出3引脚。由数字电路控制|
|11|Out3|连接到电机2的一端|
|12|0V|接地引脚连接到电路的接地(0V)|
|13|0V|接地引脚连接到电路的接地(0V)|
|14|Out4|连接到电机2的另一端|
|15|In4|直接控制输出4引脚，由数字电路控制|
|16|+V|连接到+ 5V以启用IC功能|

4.项目电路图和接线图：

![](media/40a4235ff016ce29140f3c7cedab4610.png)

![](media/272dd53c27d3abc9396d7dbde384ff5f.png)

5.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
18：小风扇”。并鼠标左键双击“Project_18\_ Small_Fan.py”。

![](media/215f8638932a3d750ba07a84f801b7eb.png)

6.项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/dc548ecd54c68b1d4fd2c29043e9b743.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：小风扇先逆时针转5秒，停止2秒，再顺时针转5秒，停止2秒，以此规律重复执行。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/229d84782825faf2dd3cdf6a7c56759e.png)

### 项目 19：舵机

1.  项目介绍：

舵机是一种可以非常精确地旋转的电机。目前已广泛应用于玩具车、遥控直升机、飞机、机器人等领域。在这个项目中，我们将使用树莓派Pico板控制舵机转动。

2.  项目元件：

|![](media/b18fe281156b29c44796f72222718d58.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|
|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|
|![](media/cd0bc424e9916881a1a903793821a042.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|舵机*1|USB 线*1|

3.  元件知识：

舵机：

![](media/99830768916233a9c5900ac399006c17.png)

舵机是一种位置伺服的驱动器，主要是由外壳、电路板、无核心马达、齿轮与位置检测器所构成。其工作原理是由接收机或者单片机发出信号给舵机，其内部有一个基准电路，产生周期为20ms，宽度为1.5ms
的基准信号，将获得的直流偏置电压与电位器的电压比较，获得电压差输出。经由电路板上的IC
判断转动方向，再驱动无核心马达开始转动，透过减速齿轮将动力传至摆臂，同时由位置检测器送回信号，判断是否已经到达定位。适用于那些需要角度不断变化并可以保持的控制系统。当电机转速一定时，通过级联减速齿轮带动电位器旋转，使得电压差为0，电机停止转动。一般舵机旋转的角度范围是0度到180
度。

控制舵机的脉冲周期为20ms，脉冲宽度为0.5ms ~ 2.5ms，对应位置为-90°~
+90°。下面是以一个180°角的舵机为例：

![](media/708316fde05c62113a3024e0efb0c237.jpeg)

伺服电机有多种规格，但它们都有三根连接线，分别是棕色、红色、橙色(不同品牌可能有不同的颜色)。棕色为GND，红色为电源正极，橙色为信号线。

![](media/3f5bc31305e64108bed3b3619d602891.jpeg)

4.  项目接线图：

舵机供电时请注意，电源电压应为3.3V-5V。请确保在将舵机连接到电源时不会出现任何错误。

![](media/4c7d70f701ec116ac4195faf3a9e545e.png)

5.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
19：舵机”。选择“myservo.py”，右击鼠标选择“Upload to
/”，等待“myservo.py”被上传到Raspberry Pi Pico，然后鼠标左键双击“Project_19_Servo_Sweep.py”。

![](media/98c9dab4e2da4d70f0548084a0e7514e.png)

![](media/9fbd6d4ea77123cc21cefbeae2668f97.png)

6. 项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/fd10ba0be5da1b901ca0070a2427f016.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：舵机将从0°旋转到180°，然后反转方向使其从180°旋转到0°，并在一个无限循环中重复这些动作。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/7ea5fe6df8d987997bcff781d6682cce.png)

![](media/c5250405a4290ecb2d758ff1097310c7.png)

### 项目 20：步进电机

1.  项目介绍：

步进电机定位准确，是工业机器人、3D打印机、大型车床等机械设备中最重要的部件。在这个项目中，我们将使用树莓派Pico板控制ULN2003步进电机驱动板来驱动步进电机转动。

2.  项目元件：

|![](media/e4d763773ba5bc91a3df128e040f491e.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/52227712f82a477e2c6abfad08529e93.png)|
|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|ULN2003步进电机驱动板*1|
|![](media/8ebb14a35091dc8d02d95cb6748dd1e9.png)|![](media/df84a18afd8b37097c469ae3ac208bc4.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|步进电机*1|母对母杜邦线若干|USB 线*1|

3.  项目知识：

![](media/8ebb14a35091dc8d02d95cb6748dd1e9.png)

步进电机：是由一系列电磁线圈控制的电机。它可以根据需要旋转精确的度数(或步数)，允许你将它移动到一个精确的位置并保持该位置。它是通过在很短的时间内为电机内部的线圈供电来做到这一点的，但你必须一直为电机供电，以保持它在你想要的位置。有两种基本类型的步进电机，单极步进和双极步进。在本项目中，我们使用的是单极步进电机28-BYJ48。

![](media/78276dc113309152d542fc3f06a24757.png)

28BYJ-48步进电机工作原理：

步进电机主要由定子和转子组成，定子是固定不动的，如下图绕着A、B、C、D线圈组的部分，线圈组导通电就会产生磁场；转子就是转动的部分，如下图定子中间的部分，两极是永磁铁。

![](media/32748e0804b1fff434181cb228b23242.png)

单步4节拍的转动原理：开始A组线圈导通，转子两极正对着A组线圈；接着A组线圈断开，B组线圈导通，转子就会顺时针转到B组线圈，转子转了一步；B断开，C导通，转子转到C组；C断开，D导通，转子转到D组；D组断开，A组导通，转子转到A组线圈。这样转子就转了半圈180度，接着再重复一次，B-C-D-A，转子转回到A组线圈，这样转子就转了一圈，总共转动了8步。如下图所示，这就是步进电机单节拍转动的原理A -
B - C - D - A ....。

如果想让步进电机逆时针转动，那只要把节拍顺序反过来就行，D - C - B - A -
D .....。

![](media/b8ae50bbdee2dd5bc683e8c450baee6a.png)

半步8节拍转动原理：8节拍，采用的是单双拍的形式，A - AB - B - BC - C -
CD - D - DA - A ......
，这样运转一拍，转子只会转动半步，例如，A组线圈导通，转子转到正对着A组线圈；接着A和B组一起导通，这样产生的磁场最强的地方在AB组线圈中间，转子两极就会转到AB组线圈中间，也就是顺时针转了半步。

步进电机参数：

我们所提供的步进电机需要转动32步，转子才能转一圈，还经过了1:64的减速齿轮组带动输出轴，这样输出轴转动一圈需要：
32 \* 64 = 2048 步。

电压5V，4相步进电机 ，4节拍模式的步进角为11.25，
8节拍模式步进角为5.625， 减速比为1:64

ULN2003步进电机驱动板：ULN2003型步进电机驱动器，将微弱信号转换为更强的控制信号，从而驱动步进电机。

下面的原理图显示了如何使用ULN2003步进电机驱动板接口将一个单极步进电机接到Raspberry Pi Pico的引脚上，并显示了如何使用四个TIP120的接口。

![](media/6fa632d2b70e97dd55565d23ec15d245.png)

4.  项目原理图和接线图：

![](media/81301873ba52d2319b71fc3e61ff7d5d.png)

![](media/b9751d6689231336b15e7993995da032.png)

5.项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
20：步进电机”。并鼠标左键双击“Project_20_Stepping_Motor.py”。

![](media/4aebdce7116d6757efa76544ad83c110.png)

6.项目结果：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/39c1d69328d82fa9f8df3ba4f85ee5b4.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：ULN2003驱动模块上的D1,D2,D3,D4四个LED点亮，步进电机先顺时针旋转，再逆时针旋转，并保持此状态循环。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/d55ffefc2932b9a0a9310baac1d84b73.png)

![](media/8dc4a0547390e0108c3960c31d330ee7.png)

### 项目 21：继电器

1.项目介绍：

在日常生活中，我们一般使用交流来驱动电气设备，有时我们会用开关来控制电器。如果将开关直接连接到交流电路上，一旦发生漏电，人就有危险。从安全的角度考虑，我们特别设计了这款具有NO(常开)端和NC(常闭)端的继电器模块。在这节课我们将学习一个比较特殊，好用的开关，就是继电器模块。

2.项目元件：

|![](media/5207588df3059cf385957664d41e9ac6.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/c141037e768eebd697ea07520708ee47.png)|![](media/ebfacf0e05bcd3941fe3b641935756b0.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|-|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|继电器模块*1|3Pin 杜邦母单*1|USB 线*1|

3.元件知识：

继电器：是用小电流去控制大电流运作的一种“自动开关”。

输入电压：3.3V-5V

额定负载：5A 250VAC (NO/NC) 5A 24VDC (NO/NC)

额定负载的意思是，可以使用微型控制器的3.3V-5V控制直流电压24V或者交流电压250V的设备。

继电器原理图：

![](media/be1c90d2b52fc2489590e3f702a087bf.emf)

4.  项目接线图：

![](media/5f8b3dfaee621c787083664297b7e094.png)

![](media/33bc9c0cb70b5b4edeb12b8326ab02a9.png)

5.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
21：继电器”。并鼠标左键双击“Project_21_Relay.py”。

![](media/53305fb958da5a9ae9660125d156586c.png)

6.  项目结果：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/f43b023e6d30e6abb2689de87c90ee45.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：继电器将循环开与关，开启1秒，关闭1秒。同时可以听到继电器开与关的声音，还可以看到继电器上的指示灯指示状态的变化。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/57a127034e23b8fc06f5615617c70484.png)

### 项目 21：调光灯

1.  项目介绍：

电位器是一个带有滑动或旋转触点的三端电阻器，它形成一个可调的分压器。它的工作原理是在均匀电阻上改变滑动触点的位置。在电位器中，整个输入电压被施加到电阻的整个长度上，输出电压是固定触点和滑动触点之间的电压值。在这个项目中，我们将学习使用树莓派Pico板读取电位器的值，并结合LED制作一个调光灯。

2.  项目元件：

|![](media/b1265f71184b5d144248ea3e847a18c9.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/03ab81e8b4f09287d2781ef0fd297f85.png)|![](media/ef77f5a64c382157fc2dea21ec373fef.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|可调电位器*1|红色 LED*1|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/845d05a6108b1662b828610ba9dcb788.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|面包板*1|220Ω电阻*1|公对母杜邦线若干|USB 线*1|

3.  元件知识：

![](media/03ab81e8b4f09287d2781ef0fd297f85.png)

可调电位器：可调电位器是电阻和模拟电子元件的一种，具有0和1两种状态(高电平和低电平)。模拟值不同，其数据状态呈现为1
~ 1024等线性状态。

4.  读取电位器的ADC值和电压值：

我们将电位器连接到树莓派Pico板的模拟IO口上来读取电位器的ADC值和电压值。接线请参照以下接线图：

![](media/fb36b9b05a5082fe9255b42eb90cf330.png)

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
22：调光灯”。并鼠标左键双击“Project_22.1_Read_Potentiometer_Analog_Value.py”。

![](media/e55aca4ad3ded1f924bb79390fe2a977.png)

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/d78e288ebb6e499647db50fabd352f5f.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：Thonny IDE下的“Shell”窗口将打印出电位器的ADC值和电压值，转动电位器手柄时，ADC值和电压值发生变化。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/4cab12c9539a2db0a42500b592dd6a0f.png)

![](media/969b9de3cf505f05d6a9361286cef9c9.png)

5.  调光灯的电路图和接线图：

在前面一步，我们读取了电位器的ADC值和电压值，现在我们需要将电位器的ADC值转换成LED的亮度，来做成一个亮度可调的灯。见如下所示接线图：

![](media/f13f9ab55497276e4323ca97479cb69b.png)

![](media/b08506476d0321b6040e38ce2992f775.png)

6.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
22：调光灯”。并鼠标左键双击“Project_22.2_Dimming_Light.py”。

![](media/1999aa847fcf2d07a7160e02e9e5bdba.png)

7.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/f2054bf619dfc67112112c294dd44493.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：转动电位器手柄，LED的亮度会相应地改变。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/325ac8e29034a452aeb457172e333306.png)

![](media/eca30dead3f4923afa0dcb0306db2319.jpeg)

### 项目 23：火焰警报器

1.  项目介绍：

火灾是一种可怕的灾害，火灾报警系统在房屋，商业建筑和工厂中是非常有用的。在本项目中，我们将使用树莓派Pico板控制火焰传感器，蜂鸣器和LED来模拟火灾报警装置。这是一个有意义的创客活动。

2.  项目元件：

|![](media/f70a6a892505b1816d151452b9b995a7.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/a50ec3e38adf10643eafac8cb62bec8a.png)|![](media/ef77f5a64c382157fc2dea21ec373fef.png)|![](media/4b4f653a76a82a3b413855493cc58fba.png)|
|-|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|火焰传感器*1|红色 LED*1|有源蜂鸣器*1|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/845d05a6108b1662b828610ba9dcb788.png)|![](media/b395b1cd2678f87b3a34dec15659efbc.png)|![](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|面包板*1|220Ω电阻*1|10KΩ电阻*1|跳线若干|USB 线*1|
|![](media/9197d4aff9356c585b7ef68e33a6881d.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|||
|NPN型晶体管(S8050)*1|1kΩ电阻*1|公对母杜邦线若干|||

3.  元件知识：

![](media/a50ec3e38adf10643eafac8cb62bec8a.png)

火焰会发出一定程度的IR光，这种光人眼是看不到的，但我们的火焰传感器可以检测到它，并提醒微控制器（如树莓派Pico板）已经检测到火灾。它有一个专门设计的红外接收管来探测火焰，然后将火焰亮度转换为波动水平信号。接收三极管的短引脚是负极，另一个长引脚是正极。我们应该连接短引脚（负极)到5V，连接长引脚(正极)到模拟引脚，一个电阻和GND。如下图所示：

![](media/3f0435fdd13d8f1845a04014709d0f41.jpeg)

注意：火焰传感器应避开日光、汽车头灯、白炽灯直接照射，也不能对着热源(如暖气片、加热器)或空调，以避免环境温度较大的变化而造成误报。同时还易受射频辐射的干扰。

4.  读取火焰传感器模拟值：

我们首先用一个简单的代码来读取火焰传感器的模拟值，并将其打印出来。接线请参照以下接线图：

![](media/2b4e0cf420a0a94d6dfdd184f06fae33.png)

![](media/87ee33681081148ff7b4e8f6ed485833.png)

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
23：火焰警报器”。并鼠标左键双击“Project_23.1_Read_Analog_Value.py”。

![](media/8da35beca986dd23a85cb6b2393f6291.png)

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/92ec7f462e7cbea4f8b7f2d6c6e3ea2c.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：Thonny IDE下的”Shell”窗口将打印火焰传感器读取的模拟值，当火焰靠近火焰传感器时，模拟值增大；反之，模拟值减小。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/547845e93ecf330ad2f7bd7d7b317475.png)

![](media/7c04b9dd8c4a10e7b9788ecd95eeeeaa.png)

5.  火焰报警的电路图和接线图：

接下来，我们将使用火焰传感器和蜂鸣器、LED制作一个有趣的项目——火灾报警装置。当火焰传感器检测到火焰时，LED闪烁，蜂鸣器报警。

![](media/2f4b0e24a35b7e5b90e7577bd4fa13b5.png)

![](media/897914ede2a0a221bff1da80d7ead221.png)

6.  项目代码：（注意：![](media/40a3ea572836945268b22dfc0cce29c3.png)代码中的阀值500可以根据实际情况自己重新设置）

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
23：火焰警报器”。并鼠标左键双击“Project_23.2_Flame_Alarm.py”。

![](media/4b866fd22c2044826871f674bf22b866.png)

7.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/76c37e6769223868d9ba389216d644d4.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：当火焰传感器检测到火焰时，LED闪烁，蜂鸣器报警；否则，LED不亮，蜂鸣器不响。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/119a3b373370c56d72b6ffb979a5c9f7.png)

### 项目 24：小夜灯

1.项目介绍：

传感器或元件在我们的日常生活中是无处不在的。例如，一些公共路灯在晚上会自动亮起，而在白天会自动熄灭。为什么呢?
事实上，这些都是利用了一种光敏元件，可以感应外部环境光强度的元件。晚上，当室外亮度降低时，路灯会自动打开；到了白天，路灯会自动关闭。这其中的原理是很简单的，在本实验中我们使用树莓派Pico板控制LED就来实现这个路灯的效果。

2.  项目元件：

|![](media/f70a6a892505b1816d151452b9b995a7.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/9e553e75b6f976f33438171eb2f2e775.png)|![](media/ef77f5a64c382157fc2dea21ec373fef.png)|![](media/b395b1cd2678f87b3a34dec15659efbc.png)|
|-|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|光敏电阻*1|红色 LED*1|10KΩ电阻*1|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|![](media/845d05a6108b1662b828610ba9dcb788.png)|
|面包板*1|公对母杜邦线若干|跳线若干|USB 线*1|220Ω电阻*1|

3.  元件知识：

![](media/9e553e75b6f976f33438171eb2f2e775.png)

光敏电阻：是一种感光电阻，其原理是光敏电阻表面上接收亮度(光)降低电阻，光敏电阻的电阻值会随着被探测到的环境光的强弱而变化。有了这个特性，我们可以使用光敏电阻来检测光强。光敏电阻及其电子符号如下：

![](media/7d575da675a2f6cb511d28b801e2abaa.png)

下面的电路是用来检测光敏电阻电阻值的变化：

![](media/5a7f7e641eb78007760a94151c1d80a5.png)

在上述电路中，当光敏电阻的电阻因光强的变化而改变时，光敏电阻与电阻R2之间的电压也会发生变化。因此，通过测量这个电压就可以得到光的强度。

4.  读取光敏电阻的模拟值：

我们首先用一个简单的代码来读取光敏电阻模拟值，并将其打印出来。接线请参照以下接线图：

![](media/68337a2b734098f3bf0ad3fe5409dd2c.png)

![](media/f959367212742f632f48c79543e74c48.png)

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
24：小夜灯”。并鼠标左键双击“Project_24.1_Read_Photosensitive_Analog_Value.py”。

![](media/74ec6193204f80a4ae5617e05c9a1c30.png)

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/289961af83d6797c824e316f659b0509.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：Thonny IDE下的”Shell”窗口将打印光敏电阻读取的模拟值，当逐渐减弱光敏电阻所处环境中的光线强度时，模拟值逐渐增大；反之，模拟值逐渐减小。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/3acf11eae4922a2017987f5ba30ee312.png)

![](media/bbabb2d5c4a997c5024e6023cb272261.png)

5.  光控灯的电路图和接线图：

我们在前面做了一个小小的调光灯，现在我们来做一个光控灯。它们的原理是相同的，即通过Raspberry Pi Pico获取传感器的模拟值，然后调节LED的亮度。

![](media/95040188210fa3c14fd3d61c4ecaac1e.png)

![](media/d34c5f9f70d90d560be98038169c270d.png)

6.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
24：小夜灯”。并鼠标左键双击“Project_24.2_Night_Lamp.py”。

![](media/757684c716a4f2b13a6a48e07d4f8f1e.png)

7.  项目结果：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/ea6b0f713205a0113807796057182c38.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：当减弱光敏电阻所处环境中的光线强度时，LED变亮，反之，LED变暗。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/a43896cfe7e9ae922daa17e46ef2efff.png)

### 项目 25：人体感应灯

1.项目介绍：

人体感应灯一般都用在黑漆漆的楼道区域，随着科技的发展，人体感应灯的使用在我们现实生活中十分常见。小区的楼道，房间的卧室、地下城的车库、卫生间等区域都会用到人体感应灯。现实生活中的人体感应灯一般是由人体红外传感器、灯、光敏电阻传感器等组成的。

在本项目中，我们将学习如何利用人体红外传感器、LED、光敏电阻来制作一款人体感应灯。

2.  项目元件：

|![](media/f70a6a892505b1816d151452b9b995a7.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/82b6a0e286b6ca25c06c6353397bad79.png)|![](media/7eb361d680dfa351f07f8527aeb37abd.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|光敏电阻*1|红色LED*1|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/51ab4ab6eefe8ba8f66234989d5282de.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|![](media/e9a8d050105397bb183512fb4ffdd2f6.png)|
|面包板*1|220Ω电阻*1|公对母杜邦线若干|跳线若干|
|![](media/239131563f68fbf379e97d8384cf2d9b.png)|![](media/ebfacf0e05bcd3941fe3b641935756b0.png)|![](media/8cf9b1b3a5fec374cde3c5f0537567cb.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|人体红外传感器*1|3Pin 杜邦母单*1|10KΩ电阻*1|USB 线*1|

3.  项目电路图和接线图：

![](media/13089278eeceeda77e4023db7d60a29e.png)![](media/98a0ef97cf5053ad684f4197ea9f101b.png)

4.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
25：人体感应灯”。并鼠标左键双击“Project_25_Human\_ Induction_Lamp.py”。

![](media/fd852d4139c4816a48132bb655d8b660.png)

5.  项目结果：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/58d04fa6a86b82238be9d5dfb0fb52bd.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：当你的手覆盖光敏电阻的感光部分来模拟黑暗状态时，树莓派Pico板内置的LED点亮，然后用另一只手在人体红外传感器前面晃动，外接LED也点亮，而且延时几秒钟后外接LED会自动关闭，同时Thonny IDE下的”Shell”窗口将打印外接LED点亮的延时时间。如果光敏电阻的感光部分没有被覆盖，可以看到树莓派Pico板内置的LED灯熄灭了，这时候，用手在人体红外传感器前面晃动，外接LED处于熄灭状态。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/8dfc6999df24b647d0e7a100c4c0c2be.png)

![](media/af94ad9d2f008956592ee64e207aa8b5.png)

### 项目 26：摇杆控制RGB灯

1.  项目介绍：

摇杆模块是一个有两个模拟输入和一个数字输入的组件。广泛应用于游戏操作、机器人控制、无人机控制等领域。在这个项目中，我们使用树莓派Pico板和摇杆模块控制RGB。这样，你可以在实践中对摇杆模块的原理和操作有更深入的了解。 

2.  项目元件：

|![](media/b18fe281156b29c44796f72222718d58.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/43acc7d0046b997a4822d8fdab834c55.png)|
|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|摇杆模块*1|
|![](media/af749ecbde89c728a8c63e6527781cac.png)|![](media/df55621713887ca0958d5fc0cceeb4ea.png)|![](media/f1aed48e2c02214415853ad2358f3744.png)|
|RGB LED*1|5P 转杜邦母单*1|公对母杜邦线若干|
|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|![](media/e65c16153d0ca27891c8c08092d96d5a.png)|
|220Ω电阻*3|USB 线*1|面包板*1|

3.  元件知识：

![](media/43acc7d0046b997a4822d8fdab834c55.png)

摇杆模块：主要是采用PS2
手柄摇杆元件，实际上摇杆模块有3个信号端引脚，模拟3维空间，摇杆模块的引脚分别是GND、VCC、信号端（B、X、Y），其中信号端X、Y模拟空间的X轴和Y轴，控制时，模块的X、Y信号端是连接单片机模拟口，通过控制2个模拟输入值来控制物体在空间X、Y轴的坐标。信号端B模拟空间Z轴，它一般是接数字口，做按键使用。

VCC接单片机电源输出端V/VCC（3.3/5V），GND接单片机G/GND，原始状态下读出电压大约为1.65V/2.5V左右，对于X轴方向，当随箭头方向逐渐按下，读出电压值随着增加，且可以达到最大电压，随箭头相反方向逐渐按下，读出电压值逐渐减少，减少到最小电压；对于Y轴方向，当沿着模块上的箭头方向逐渐按下，读出电压值逐渐减少，减少到最小电压，随箭头相反方向逐渐按下，读出电压值随着增加，且可以达到最大电压；对于Z轴方向，信号端B接数字口，原始状态下输出0，按下输出1。这样，我们可以读取两个模拟值和一个数字口的高低电平情况，判断模块上摇杆的工作状态。

模块参数：

输入电压：DC 3.3V ~ 5V

输出信号：X/Y双轴模拟值+Z轴数字信号

适用范围：适用于控制点坐标在平面内的运动，双自由度舵机的控制等。

产品特点：外观精美，摇杆手感优越，操作简单，反应灵敏，使用寿命长。

4.  读取摇杆模块的值：

我们必须使用树莓派Pico板的模拟IO口从摇杆模块的X/Y引脚读取模拟值，并使用数字IO口读取按钮的数字信号。请按照下面的接线图进行接线：

![](media/80c2deff4678a08725e0df9c3465db91.png)

![](media/bbcd8beb3a10e0f5d73dbd527b9dc0f1.png)

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
26：摇杆控制RGB灯”。然后鼠标左键双击“Project_26.1_Read_Rocker_Value.py”。

![](media/0d5b79e8e898efe4dc12bf3c8bcc4aaf.png)

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/d4f5a7323a71eb46f3807ace94feadf7.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：Thonny IDE下的”Shell”窗口将打印当前摇杆的模拟值和数字值，移动摇杆或按下它将改变”Shell”中的模拟值和数字值。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/9278662225e99e6c2d84abb8da9b81ba.png)

![](media/fc2b5c16e690a43bb7a5edf08483e614.png)

![](media/237c70493a9d044cf5d2f823359fc0a6.png)

5.  摇杆模块控制RGB的电路图和接线图：

我们刚读了摇杆模块的值，这里我们需要用摇杆模块和RGB做一些事情，按照下图连接：

![](media/7e37e804327c10abce60756f6bb5cb3a.png)

![](media/4924a62ef1a0b35f3d6637a461929f03.png)

6.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
26：摇杆控制RGB灯”。然后鼠标左键双击“Project_26.2_Rocker_Control_Light.py”。

![](media/857892223acacbc47c5cb5274c0755e3.png)

7.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/e235e7e3b47aa271dbe3b5b13f419014.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：①如果摇杆在X方向上移动到最左边，RGB光变成红色;
②如果摇杆在X方向上移动到最右边，RGB光变为绿色;
③如果摇杆在Y方向上移动到最上面，RGB光变成白色;
④如果摇杆在Y方向上移动到最下面，RGB光变成蓝色。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/d47d253518eaaf65f382bde5357aef8a.png)

### 项目 27：温湿度表 

1.  项目介绍：

在冬季时，空气中的湿度很低，就是空气很干燥，再加上寒冷，人体的皮肤就容易过于干燥而裂，所以需要在用加湿器给家里的空气增加湿度，但是怎么知道空气过于干燥了呢？那就需要检测空气湿度的设备，这节课就来学习温湿度传感器的使用。我们使用温湿度传感器制作一个温湿度计，并且还结合LCD 128X32 DOT来显示温度和湿度值。

2.  项目元件：

|![](media/20244a3eedd455abdbe6dc69b0ca6b8f.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/2d013e7634507fa3570235454abcd3fc.png)|![](media/09f2e623faf741f16ba9b0390d587567.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|温湿度传感器*1|LCD 128X32 DOT*1|
|![](media/e615c2849ce15bdfc8e26432004124ec.png)|![](media/ebfacf0e05bcd3941fe3b641935756b0.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)||
|4P 转杜邦线母单10厘米*1|3Pin 杜邦母单*1|USB 线*1||

3.  元件知识：

![](media/2d013e7634507fa3570235454abcd3fc.png)

温湿度传感器：是一款含有已校准数字信号输出的温湿度复合传感器，其精度湿度±5%RH，
温度±2℃，量程湿度20-90%RH，
温度0~50℃。温湿度传感器应用专用的数字模块采集技术和温湿度传感技术，确保产品具有极高的可靠性和卓越的长期稳定性。温湿度传感器包括一个电阻式感湿元件和一个NTC测温元件，非常适用于对精度和实时性要求不高的温湿度测量场合。

工作电压在3.3V-5.5V范围内。  
温湿度传感器有三个引脚，分别为VCC，GND和S。S为数据输出的引脚。使用的是串行通讯。

温湿度传感器的单总线格式定义：

|名称|单总线格式定义|
|-|-|
|起始信号|微处理器把数据总线(SDA)拉低一段时间至少 18ms(最大不得超过30ms)，通知传感器准备数据。|
|响应信号|传感器把数据总线（SDA）拉低 83µs，再接高 87µs以响应主机的起始信号。|
|湿度|湿度高位为湿度整数部分数据，湿度低位为湿度小数部分数据|
|温度|温度高位为温度整数部分数据，温度低位为温度小数部分数据，且温度低位Bit8 为 1 则表示负温度，否则为正温度|
|校验位|校验位＝湿度高位+湿度低位+温度高位+温度低位|

温湿度传感器数据时序图：

用户主机（MCU）发送一次开始信号后，温湿度传感器从低功耗模式转换到高速模式，待主机开始信号结束

后，温湿度传感器发送响应信号，送出 40bit
的数据，并触发一次信采集。信号发送如图所示。

![](media/c3038afcfc88d77da5ce9e8facf8ef32.png)

结合代码，可以理解的更好。

温湿度传感器可以很容易地将温湿度数据添加到您的DIY电子项目中。它是完美的远程气象站，家庭环境控制系统，和农场或花园监测系统。

温湿度传感器的参数：

工作电压：+5 V

温度范围：0-50 °C ，误差：± 2 °C

湿度范围：20-90% RH ，误差：± 5% RH

数字接口

温湿度传感器的原理图：

![](media/53fa034cbbcec22579b2bdf8252c90cd.emf)

4.  读取温湿度值：

![](media/b2e37efa629abda91234abb91f32f7ee.png)

![](media/a202b07be0cd714ca3248b71191ba176.png)

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
27：温湿度表”。选择“dht11.py”，右键单击鼠标选择 “上载到/”，等待
“dht11.py”被上传到Raspberry Pi Pico，然后鼠标左键双击“Project_27.1_Detect_Temperature_Humidity.py”。

![](media/3e818d949aae9561ed698d96678a5082.png)

![](media/32ff85e3a58ad4e50c3f05962b877ca2.png)

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/a99d23fc37da9015cff8f657ac46535f.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：Thonny IDE下的”Shell”窗口将打印当前显示当前环境中的温湿度数据，如下图。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/62c81990f399ad34585e5e4a06ea4f1d.png)

![](media/af350892cefaa74dae1740153a0c1626.png)

5.  温湿度仪表的电路图和接线图：

现在我们开始用LCD_128X32_DOT打印温湿度传感器的值，我们会在LCD_128X32_DOT的屏幕上看到相应的值。让我们开始这个项目吧。请按照下面的接线图进行接线：

特别注意：这里必须使用4P
转杜邦线母单10厘米连接LCD_128X32_DOT，LCD_128X32_DOT才会显示正常；否则，使用4P
转杜邦线母单20厘米，LCD_128X32_DOT可能会显示不正常。

![](media/beb75f9b8c582b57cb5846535f0575a2.png)

![](media/018d4ef8b56b679b71d1f2af5a907d84.png)

6.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
27：温湿度表”。分别选择“dht11.py”,“lcd128_32.py”和
“lcd128_32_fonts.py”，右键单击鼠标选择 “上载到/”，等待
“dht11.py”，“lcd128_32.py”和 “lcd128_32_fonts.py”被上传到Raspberry Pi Pico，然后鼠标左键双击“Project_27.2_Temperature_Humidity_Meter.py”。

![](media/3e818d949aae9561ed698d96678a5082.png)

![](media/8b52410fb6c0d7e4800799a9715bdb38.png)

![](media/01fd7f40b3c62ea46ed6dd849b099505.png)

![](media/1998e8949d5147375f656652ad459425.png)

7.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/e4e86c17190ace321e128be5a6e8226e.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：LCD 128X32 DOT的屏幕上显示温湿度传感器检测环境中相应的温度值和湿度值。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/25a9c9eb5bda3d24d710777ad6f6d206.png)

### 项目 28：测距仪表

1. 项目介绍：  
HC-SR04超声波传感器是一种非常实惠的距离传感器，主要用于各种机器人项目中的物体躲避。它也被用于水位传感，甚至作为一个停车传感器。我们把超声波传感器当作蝙蝠的眼睛，在黑暗中，蝙蝠仍然可以通过超声波识别前方的物体和方向。在本项目中，我们使用树莓派Pico板控制超声波传感器和LED模拟超声波测距仪。

2. 项目元件：

|![](media/ea74681ffd2116a2434692d34c25e829.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/11163a0fe0cd3efaf4ccd57fb237f103.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|超声波传感器*1|公对母杜邦线若干|
|![](media/e615c2849ce15bdfc8e26432004124ec.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/7eb361d680dfa351f07f8527aeb37abd.png)|
|4P 转杜邦线母单20厘米*1|220Ω电阻*4|跳线若干|红色LED*4|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|||
|面包板*1|USB 线*1|||

3.  元件知识：

HC-SR04超声波传感器：像蝙蝠一样使用声纳来确定与物体的距离，它提供了精准的非接触范围检测，高精度和稳定的读数。它的操作不受阳光或黑色材料的影响，就像精密的照相机(在声学上像布料这样比较软的材料很难被探测到)。它带有超声波发射器和接收器。

![](media/653a2e40ce31d039c801edce1050114d.png)

在超声波传感器的前面是两个金属圆筒，这些是转换器。转换器将机械能转换成电信号。在超声波传感器中，有发射转换器和接收转换器。发射转换器将电信号转换为超声波脉冲，接收转换器将反射的超声波脉冲转换回电信号。如果你看超声波传感器的背面，你会看到的发射转换器后面有一个IC。这是控制发射转换器的IC。在接收转换器后面也有一个IC，这是一个四运算放大器，它将接收转换器产生的信号放大成足以传输到微控制器的信号。

时序图：

图示HC-SR04的时序图。为了开始测量，SR04的Trig必须接受至少10us的高(5V)脉冲，这将启动传感器将发射出8个周期的40kHz的超声波脉冲，并等待反射的超声波脉冲。当传感器从接收器检测到超声波时，它将设置回波引脚为高(5V)和延迟一个周期(宽度)，与距离成比例。为了获得距离，测量Echo引脚的宽度。

![](media/ba43be6007d9fe3aab0bb609868af640.png)

时间=回波脉冲宽度，单位为us(微秒)

距离厘米=时间/ 58

距离(英寸)=时间/ 148

4.  读取超声波传感器距离值

我们将从一个简单的超声波测距开始，并打印测量的距离。

![](media/8835e046cfb2a4b1d6da5e78c473ccce.png)

HC-SR04超声波传感器有四个引脚：Vcc、Trig、Echo和GND。Vcc引脚提供产生超声波脉冲的电源，接Vcc/+5V。GND引脚接地/GND。Trig引脚是控制板发送信号来启动超声波脉冲的地方。Echo引脚是超声波传感器向控制板发送关于超声波脉冲行程持续时间的信息的地方。按下图接线：

![](media/9b58d226f676712f774b55978a89938c.png)

![](media/477cc941c0c2ad711a6b326f441c49e9.png)

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
28：测距仪表”。并鼠标左键双击“Project 28.1_Ultrasonic_Ranging.py”。

![](media/994f0ba8de32d7683496dbdda5d6c238.png)

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/81f234078e0c4cfdd981ed5802a39c22.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：Thonny IDE下的”Shell”窗口将打印超声波传感器和物体之间的距离值。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/5dadf132255a4a7911743aa424a8aa00.png)

![](media/ce873cf513307a15f9aa58078c8dd7d6.png)

5.  超声波测距仪的电路图和接线图：

接下来，我们将使用树莓派Pico板控制超声波传感器和4个LED模拟超声波测距仪。按如下图接好线：

![](media/bf201b7c14c97e201dadcb24c687d3d5.png)

![](media/6596aa78b3aceb528058e22b3a26ed52.png)

6.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
28：测距仪表”。并鼠标左键双击“Project_28.2_Ultrasonic_Ranger.py”。

![](media/200fe5080229725be97da84dc8f6ae84.png)

7.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/2a10650828abccc1202ce0d8440ec5be.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：Thonny IDE下的”Shell”窗口将打印超声波传感器和物体之间的距离值，另外，当我们用手在超声波传感器前移动时，相应的LED会亮起来。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/e8c0be98ba6066c8a5756ff841f17edf.png)

### 项目 29：温度仪表

1.  项目介绍：

热敏电阻是一种电阻，其阻值取决于温度和温度的变化，广泛应用于园艺、家庭警报系统等装置中。因此，我们可以利用这一特性来制作温度计。

2.  项目元件：

|![](media/8f45d8141f23885af95f870ab64a859c.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|
|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|公对母杜邦线若干|
|![](media/06b78e3697de1bb564b007ebdcf0581b.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/b45bb81bb3763377c63accce606ac5f2.png)|
|LCD_128X32_DOT*1|面包板*1|热敏电阻*1|
|![](media/e615c2849ce15bdfc8e26432004124ec.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|![](media/b395b1cd2678f87b3a34dec15659efbc.png)|
|4P 转杜邦线母单10厘米*1|USB 线*1|10KΩ电阻*1|

3.  元件知识：

热敏电阻：热敏电阻是一种温度敏感电阻。当热敏电阻感应到温度的变化时，它的电阻就会发生变化。我们可以利用热敏电阻的这种特性来检测温度强度。热敏电阻及其电子符号如下所示。

![](media/809b8634747fb295021f12e3b92b7894.png)

热敏电阻的电阻值与温度的关系为：

![](media/04312ac83502354f253ae6cba9f005dd.wmf)

式中：

Rt为热敏电阻在T2温度下的电阻；

R为热敏电阻在T1温度下的标称阻值；

EXP\[n\]是e的n次幂；

B为温度指数；

T1，T2是开尔文温度(绝对温度)，开尔文温度=273.15     +摄氏温度。对于热敏电阻的参数，我们使用：B=3950,     R=10KΩ，T1=25℃。热敏电阻的电路连接方法与光敏电阻类似，如下所示：

![](media/ac0d68aac58bffa5c99e1d0ed3a8bc37.jpeg)

我们可以利用ADC转换器测得的值来得到热敏电阻的电阻值，然后利用公式来得到温度值。因此，温度公式可以推导为：

![](media/7d6cc89970b6158b40707eb7b5d3b0d5.wmf)

4.  读取热敏电阻的值：

首先我们学习热敏电阻读取当前的ADC值、电压值和温度值，并将其打印出来。请按下面的接线图接好线：

![](media/d1cc8f28e153531547d11ea977c37eca.png)

![](media/934f77b466c3f5391233dbbe62afecd6.png)

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
29：温度仪表”。并鼠标左键双击“Project_29.1_Read_the_thermistor_analog_value.py”。

![](media/24ed370a6a75cd028645297b602ec560.png)

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/69f090a32bc632d042b39232d646f110.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：Thonny IDE下的”Shell”窗口将不断显示热敏电阻当前的ADC值、电压值和温度值。试着用食指和拇指捏一下热敏电阻(不要碰触导线)一小段时间，你应该会看到温度值增加。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/95201a96c05b024f9d9f2e45f70c5d32.png)

![](media/0a035900fbc73a112eced64a926872ad.png)

5.  温度仪表电路图和接线图：

特别注意：这里必须使用4P     转杜邦线母单10厘米连接LCD_128X32_DOT，LCD_128X32_DOT才会显示正常；否则，使用4P     转杜邦线母单20厘米，LCD_128X32_DOT可能会显示不正常。

![](media/458af2aaa2a441e37e460179529084f7.png)

![](media/954828a7a1afd281d2b8a2a702cf1e83.png)

6.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
29：温度仪表”。分别选择“lcd128_32.py”和
“lcd128_32_fonts.py”，右键单击鼠标选择 “上载到 /”，等待“lcd128_32.py”和
“lcd128_32_fonts.py”被上传到Raspberry Pi Pico。并鼠标左键双击“Project_29.2_Temperature_Instrument.py”。

![](media/eb05ffb074c3b961ebb0bcf6345ad20b.png)

![](media/fd152ef52c3825853bd716f5e29b7626.png)

![](media/ab1da39cbf083a5f2af913e1bfe7eca8.png)

7.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/1e4abc0fee252d1c9e671110a14cb8af.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：LCD 128X32 DOT的屏幕上显示热敏电阻的电压值和当前环境中的温度值。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/e4bb45f1a801d469aa873b0bece4fd9a.png)

### 项目 30：键盘控制门

1. 项目介绍：

常用的数字按钮传感器，一个按钮就使用一个IO口，而有时我们需要的按钮比较多时，就会占用过多的IO口，为了节省IO口的使用，把多个按钮做成了矩阵类型，通过行列线的控制，实现少IO口控制多个按钮。在本项目中，我们将来学习树莓派Pico板和薄膜4\*4矩阵键盘控制舵机和蜂鸣器。

2.  项目元件：

|![](media/7db4bbca6a859c37ae9bfdb52b676bb8.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/cd0bc424e9916881a1a903793821a042.png)|![](media/4b4f653a76a82a3b413855493cc58fba.png)|
|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|舵机*1|有源蜂鸣器*1|
|![](media/fcd187eb009098d691927511606c991b.jpeg)|![](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)|
|薄膜4*4矩阵键盘*1|跳线若干|面包板*1|公对母杜邦线若干|
|![](media/9197d4aff9356c585b7ef68e33a6881d.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)||
|NPN型晶体管(S8050)*1|1kΩ电阻*1|USB 线*1||

3.  元件知识：

4\*4矩阵键盘：键盘是一种集成了许多键的设备。如下图所示，一个4x4键盘集成16个键。

![](media/fcd187eb009098d691927511606c991b.jpeg)

与LED矩阵集成一样，在4x4键盘中，每排键都是用一根引脚连接，每一列键都是一样的。这样的连接可以减少处理器端口的占用。内部电路如下所示。

![](media/5ebdacba906622079e0ef41dc1ea3fdf.png)

使用方法类似于矩阵LED，即使用行扫描或列扫描方法检测每列或每行上的键的状态。以列扫描法为例，向第4列(Pin4)发送低电平，检测第1、2、3、4行电平状态，判断A、B、C、D键是否按下。然后依次将低电平发送到列3、2、1，检测是否有其它键被按下。然后，你可以获得所有键的状态。

4.  读取4\*4矩阵键盘的键值：

我们首先使用一个简单的代码读取4\*4矩阵键盘的键值，并将其打印出来，其接线图如下所示：

![](media/29629f4ded6b09ca14050716373dcf26.png)![](media/e7f75540c95c680f6ef9b70704a5cafb.png)

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
30：键盘控制门”。 选择“keypad.py”，右键单击鼠标选择 “上载到/”，等待
“keypad.py”被上传到Raspberry Pi Pico，然后鼠标左键双击“Project_30.1_4x4_Matrix_Keypad_Display.py”。

![](media/e09ad12dd731e66130850d71b90a495d.png)

![](media/8bc48c9658427efa4fcd02fc47e5164c.png)

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/2ecc5f1371eae534cc9b7d4d87e9edc2.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：按下键盘，Thonny IDE下的”Shell”窗口将打印对应的键值，如下图所示。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/c80c1f6bba203f9f875c59a699c94014.png)

![](media/2f82f861d68daaaad8085b6a1bcc2e8d.png)

5.  Keypad Door的电路图和接线图：

在上一实验中，我们已经知道了4\*4矩阵键盘的键值，接下来，我们使用4\*4矩阵键盘作为键盘来控制舵机和蜂鸣器。

![](media/a3ff2cd6ff82ae35f18f335eda545656.png)

![](media/ff4c106ffcb5041252558ceef89c4006.png)

6.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
30：键盘控制门”。 分别选择“keypad.py”和 “myservo.py”，右键单击鼠标选择
“上载到 /”，等待 “keypad.py”和“myservo.py”被上传到Raspberry Pi Pico，然后鼠标左键双击“Project_30.2_Keypad_Door.py”。

![](media/e09ad12dd731e66130850d71b90a495d.png)

![](media/cee574f952b57a4e79bb557535d6d984.png)

![](media/ce190c8d3fd29f663ce4112643eed67c.png)

7.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/0ef1e93ca4f7ee7ae7e1625f0614d052.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：按键盘输入4个字符的密码，如果输入正确（正确密码：1234），舵机会转动一定角度，然后回到原来的位置。如果输入错误，将发出输入错误警报。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/3e0877d98712b6126da73f5632c2ef0a.png)

![](media/d45bd766b2b2630219f8bef283a07417.png)

### 项目 31：红外遥控控制声音和LED

1.  项目介绍：

红外遥控是一种低成本、易于使用的无线通信技术。IR光与可见光非常相似，除了它的波长稍长一点。这意味着红外线是人眼无法检测到的，这对于无线通信来说是完美的。例如，当你按下电视遥控器上的一个按钮时，一个红外LED会以每秒38000次的频率反复开关，将信息(如音量或频道控制)传送到电视上的红外感光器。

我们将首先解释常见的红外通信协议是如何工作的。然后我们将从一个遥控器和一个红外接收组件开始这个项目。

2.  项目元件：

|![](media/17098ffd05750eb6b34eb75b82fbb37a.jpeg)|![](media/2762753d227ba94de9f6e5c9ff79fe53.png)|![](media/88e6b057fb4b0c576c9b2111d15b26e5.png)|![](media/f1a86fc81ab4b043263ce7e01e14d470.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|
|-|-|-|-|-|
|树莓派Pico板*1|树莓派Pico板的扩展板*1|红外接收器 *1|RGB LED*1|220Ω电阻*3|
|![](media/31ab42dc405244fa383c76b57538a6cb.png)|![](media/d1ea1bb2b2749820cab389d5b85b838b.png)|![](media/a22dac8c5edbe90e867cbb04769d1816.png)|![](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|
|红外遥控器*1|无源蜂鸣器*1|10KΩ电阻*1|跳线若干|USB 线*1|
|![](media/e380dd26e4825be9a768973802a55fe6.png)|![](media/9197d4aff9356c585b7ef68e33a6881d.png)|![](media/098a2730d0b0a2a4b2079e0fc87fd38b.png)|![](media/3ac518b4caa5086041545c60c7a6a2d1.png)||
|面包板*1|NPN型晶体管(S8050)*1|1kΩ电阻*1|公对母杜邦线若干||

3.  元件知识：

红外(IR)遥控器：是一种具有一定数量按钮的设备。按下不同的按钮会使位于遥控器前端的红外发射管以不同的编码发送红外信号。红外遥控技术应用广泛，如电视、空调等。因此，在当今科技发达社会，红外遥控技术使你切换电视节目和调节空调温度都很方便。

我们使用的遥控器如下所示：

该红外遥控器采用NEC编码，信号周期为110ms。

![](media/28c0a8a6423fa66794502e6db19f997d.jpeg)

红外(IR)接收器：它是一种元件，可以接收红外光，所以可以用它来检测红外遥控器发出的红外光信号。红外接收器解调接收到的红外光信号，并将其转换回二进制，然后将信息传递给微控制器。

红外信号调制过程图：

![](media/b664b5b6884f7d3d8b4ee7eebdfd699b.png)

4.  解码红外信号：

我们按照下面接线图将红外接收元件连接到树莓派Pico板。

![](media/b9a3bd9b4366bc22d72ec6788a39e018.png)

![](media/5a132241d4bc918d86182d2a4b232ed9.png)

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
31：红外遥控控制声音和LED”。选择“irrecvdata.py”，右键单击选择
“上载到/”,等待“irrecvdata.py”被上传到Raspberry Pi Pico，然后鼠标左键双击“Project_31.1_Decoded_IR_Signal.py”。

![](media/02ffa3f6b12fbbc516e0d71ac2d44f4e.png)

![](media/59c70585146fe756526d36d4e747021f.png)

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/fed4313a6a7a255472a123dd619137f2.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：将红外遥控器发射器对准红外接收头，按下红外控制器上的按键，Thonny IDE下的”Shell”窗口将打印当前接收到的按键编码值。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/317ca8b4e6a0187be5d95ee6225d8f3f.png)

![](media/623f8fa842b90a093d286954835483c6.png)

写下红外遥控器与每个按键相关联的按键编码值，因为你稍后将需要这些信息。

![](media/b5c753d6a1f5126fdd8e8423b82a836c.png)

5.  红外遥控的电路图和接线图：

![](media/779caf9e8a0bbb0ecf053fbee11ce3ec.png)

![](media/5a2531a167131af693af10189b4afe36.png)

6.  项目代码：

本项目中使用的代码保存在文件夹“3. Python 教程\1. Windows 系统\2.
项目课程”中。你可以把代码移到任何地方。例如，我们将“2.
项目课程”文件夹保存在Disk(D)中，路径为D:\2. 项目课程。

打开“Thonny”软件，点击“此电脑”→“D:”→“2. 项目课程”→“项目
31：红外遥控控制声音和LED”。选择“irrecvdata.py”，右键单击选择
“上载到/”,等待“irrecvdata.py”被上传到Raspberry Pi Pico，然后鼠标左键双击“Project_31.2_IR_Control_Sound_And_LED.py”。

![](media/02ffa3f6b12fbbc516e0d71ac2d44f4e.png)

![](media/d9f5f098222947645e9ee7abc62ac97f.png)

7.  项目现象：

确保树莓派Pico板已经连接到电脑上，单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”。

![](media/bc2fdb431dddd419ce937db93d6195a5.png)

单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”，代码开始执行，你会看到的现象是：按红外遥控器的1~7键，可以听到do、re、mi、fa、sol、la、si
等蜂鸣器的声音，同时RGB分别亮红灯，绿灯，蓝灯，黄灯，洋红灯，蓝绿灯，白灯。按其他另一按键（除1-7键以外），蜂鸣器就停止播放，RGB熄灭。按“Ctrl+C”或单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”退出程序。

![](media/8395c806a22054e2286d84a84a90860d.png)

特别注意：当代码在运行时有时候会出现以下类似提示语，只要鼠标先单击![](media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“停止/重启后端进程”，然后再单击![](media/da852227207616ccd9aff28f19e02690.png)“运行当前脚本”就可以使代码重新运行。

![](media/3f425db5cda9eb56bc1f29c27fa6696d.png)

(注意:在使用前，我们需要将红外遥控器底部的塑料片去掉)
