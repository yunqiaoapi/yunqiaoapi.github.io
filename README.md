

# <font style="color:rgb(31, 35, 40);">Claude Code Windows版使用教程</font>
## <font style="color:rgb(31, 35, 40);">系统要求</font>
+ <font style="color:rgb(31, 35, 40);">✅</font>**<font style="color:rgb(31, 35, 40);">操作系统</font>**<font style="color:rgb(31, 35, 40);">：Windows 10 或 Windows 11（</font>**<font style="color:rgb(31, 35, 40);">必须是 64 位</font>**<font style="color:rgb(31, 35, 40);">）</font>
+ <font style="color:rgb(31, 35, 40);">✅</font>**<font style="color:rgb(31, 35, 40);">内存</font>**<font style="color:rgb(31, 35, 40);">：建议4GB以上</font>
+ <font style="color:rgb(31, 35, 40);">✅</font>**<font style="color:rgb(31, 35, 40);">硬盘空间</font>**<font style="color:rgb(31, 35, 40);">：约2-4GB</font>
+ <font style="color:rgb(31, 35, 40);">✅</font>**<font style="color:rgb(31, 35, 40);">网络</font>**<font style="color:rgb(31, 35, 40);">：需要联网进行安装和使用</font>
+ <font style="color:rgb(31, 35, 40);">✅</font>**<font style="color:rgb(31, 35, 40);">权限</font>**<font style="color:rgb(31, 35, 40);">：需要管理员权限</font>



## <font style="color:rgb(31, 35, 40);">完整安装步骤</font>
### <font style="color:rgb(31, 35, 40);">第一步：安装 Git for Windows（必需）</font>
<font style="color:rgb(89, 99, 110);">⚠️</font><font style="color:rgb(89, 99, 110);"> </font>**<font style="color:rgb(89, 99, 110);">重要</font>**<font style="color:rgb(89, 99, 110);">：Claude Code 在 Windows 上依赖 Git Bash 运行，必须先安装 Git。</font>

#### <font style="color:rgb(31, 35, 40);">1.1 下载Git</font>
<font style="color:rgb(31, 35, 40);">访问Git官网下载页面：</font>  
 [https://git-scm.com/downloads/win](https://git-scm.com/downloads/win)

<font style="color:rgb(31, 35, 40);">点击下载最新的</font>**<font style="color:rgb(31, 35, 40);">64位版本</font>**<font style="color:rgb(31, 35, 40);">。</font>



#### <font style="color:rgb(31, 35, 40);">1.2 安装Git</font>
1. <font style="color:rgb(31, 35, 40);">上部下载的安装文件（如</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">Git-2.51.2-64-bit.exe</font>`<font style="color:rgb(31, 35, 40);">）</font>
2. **<font style="color:rgb(31, 35, 40);">全程使用默认选项</font>**<font style="color:rgb(31, 35, 40);">，一路点击“Next”</font>
3. <font style="color:rgb(31, 35, 40);">确保在“调整您的PATH环境”步骤中选择：</font>
    - <font style="color:rgb(31, 35, 40);">✅</font><font style="color:rgb(31, 35, 40);"> </font>**<font style="color:rgb(31, 35, 40);">"Git from the command line and also from 3rd-party software"</font>**<font style="color:rgb(31, 35, 40);">（默认选项）</font>
4. <font style="color:rgb(31, 35, 40);">点击“安装”开始安装</font>
5. <font style="color:rgb(31, 35, 40);">完成后点击“完成”</font>

#### <font style="color:rgb(31, 35, 40);">1.3 验证Git安装</font>
1. <font style="color:rgb(31, 35, 40);">按</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">Win + R</font>`
2. <font style="color:rgb(31, 35, 40);">输入</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">cmd</font>`<font style="color:rgb(31, 35, 40);">，按回车</font>
3. <font style="color:rgb(31, 35, 40);">在命令提示符中输入</font>

<font style="color:rgb(31, 35, 40);">  git --version</font>

<font style="color:rgb(31, 35, 40);">✅</font><font style="color:rgb(31, 35, 40);"> 如果显示类似</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">git version 2.51.2.windows.1</font>`<font style="color:rgb(31, 35, 40);">，说明安装成功。</font>

<font style="color:rgb(31, 35, 40);"></font>

### <font style="color:rgb(31, 35, 40);">第二步：安装Claude代码</font>
#### <font style="color:rgb(31, 35, 40);">2.1 以管理员身份打开PowerShell</font>
1. `<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">Win</font>`<font style="color:rgb(31, 35, 40);">+Q </font>
2. <font style="color:rgb(31, 35, 40);">输入</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">powershell</font>`
3. **<font style="color:rgb(31, 35, 40);">右键</font>**<font style="color:rgb(31, 35, 40);">单击“Windows PowerShell”</font>
4. <font style="color:rgb(31, 35, 40);">选择</font>**<font style="color:rgb(31, 35, 40);">“以管理员身份运行”</font>**

#### <font style="color:rgb(31, 35, 40);">2.2 运行安装命令</font>
<font style="color:rgb(31, 35, 40);">在PowerShell中复制并运行以下命令：</font>

<font style="color:rgb(31, 35, 40);background-color:rgb(246, 248, 250);">irm https://claude.ai/install.ps1 | iex</font>

#### <font style="color:rgb(31, 35, 40);">2.3 等待安装完成</font>
<font style="color:rgb(31, 35, 40);">安装过程会显示详细信息，完成后会显示：</font>

```plain
✅ Installation complete!
Version: 2.0.34
Location: C:\Users\你的用户名\.local\bin\claude.exe
```



### <font style="color:rgb(31, 35, 40);">第三步：配置环境变量（添加PATH）</font>
<font style="color:rgb(31, 35, 40);">安装完成后需要将Claude添加到系统PATH，这样才能在任何位置运行</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">claude</font>`<font style="color:rgb(31, 35, 40);">命令。</font>

#### <font style="color:rgb(31, 35, 40);">方法一：图形界面操作（新手）</font>
1. <font style="color:rgb(31, 35, 40);">按</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">Win + R</font>`<font style="color:rgb(31, 35, 40);">，输入</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">sysdm.cpl</font>`<font style="color:rgb(31, 35, 40);">，按回车</font>
2. <font style="color:rgb(31, 35, 40);">点击</font>**<font style="color:rgb(31, 35, 40);">“高级”</font>**<font style="color:rgb(31, 35, 40);">标签</font>
3. <font style="color:rgb(31, 35, 40);">点击</font>**<font style="color:rgb(31, 35, 40);">“环境变量”</font>**<font style="color:rgb(31, 35, 40);">按钮</font>
4. <font style="color:rgb(31, 35, 40);">在</font>**<font style="color:rgb(31, 35, 40);">“用户变量”</font>**<font style="color:rgb(31, 35, 40);">区域（窗口上半部分），找到并左边</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">Path</font>`
5. <font style="color:rgb(31, 35, 40);">点击</font>**<font style="color:rgb(31, 35, 40);">“新建”</font>**<font style="color:rgb(31, 35, 40);">按钮</font>
6. <font style="color:rgb(31, 35, 40);">输入：</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">C:\Users\你的用户名\.local\bin</font>`
    - <font style="color:rgb(31, 35, 40);">将</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">你的用户名</font>`<font style="color:rgb(31, 35, 40);">替换为实际的 Windows 用户名</font>
7. <font style="color:rgb(31, 35, 40);">依次点击</font>**<font style="color:rgb(31, 35, 40);">“确定”</font>**<font style="color:rgb(31, 35, 40);">关闭所有窗口</font>

#### <font style="color:rgb(31, 35, 40);">方法二：PowerShell命令（快速）</font>
<font style="color:rgb(31, 35, 40);">在PowerShell（管理员模式）中运行：</font>

<font style="color:rgb(31, 35, 40);background-color:rgb(246, 248, 250);">[Environment]::SetEnvironmentVariable("Path", $env:Path + ";C:\Users\$env:USERNAME\.local\bin", "User")</font>

  
 

### <font style="color:rgb(31, 35, 40);">第四步：验证安装</font>
#### <font style="color:rgb(31, 35, 40);">4.1 重新启动PowerShell</font>
<font style="color:rgb(31, 35, 40);">⚠️</font><font style="color:rgb(31, 35, 40);"> </font>**<font style="color:#DF2A3F;">必须关闭所有PowerShell窗口并重新打开</font>**<font style="color:#DF2A3F;">，PATH修改才会生效。</font>

#### <font style="color:rgb(31, 35, 40);">4.2 测试命令</font>
<font style="color:rgb(31, 35, 40);">打开新的PowerShell窗口，输入：</font>

<font style="color:rgb(31, 35, 40);background-color:rgb(246, 248, 250);">claude --version</font>

<font style="color:rgb(31, 35, 40);">✅</font><font style="color:rgb(31, 35, 40);"> 如果显示版本号（如</font>`<font style="color:rgb(31, 35, 40);background-color:rgba(129, 139, 152, 0.12);">2.0.34</font>`<font style="color:rgb(31, 35, 40);">），说明安装成功！</font>

<font style="color:rgb(31, 35, 40);"></font>

### <font style="color:rgb(31, 35, 40);">第五步：配置API Key</font>
**<font style="color:rgb(38, 38, 38);">方法一（推荐）：通过JSON文件进行设置</font>****<font style="color:rgb(38, 38, 38);">配置 </font>**

##### **<font style="color:rgb(38, 38, 38);">配置 </font>**<font style="background-color:#FBDE28;">.claude.json</font>
<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/63327424/1772855385160-0ebecfbc-4bdb-4d5f-8786-ca500a0cf812.png)

<font style="color:rgb(52, 64, 84);">找到 </font><font style="color:rgb(52, 64, 84);background-color:#FBDE28;">.claude.json</font><font style="color:rgb(52, 64, 84);"> 然后双击打开文件</font>

<font style="color:rgb(52, 64, 84);">文件中开头添加以下内容：</font>

<font style="color:rgb(52, 64, 84);"> "hasCompletedOnboarding": true,</font>

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/67472675/1776657124914-cd6eaf25-2e54-4078-be8f-1738ac4c15e5.png)

**<font style="color:#DF2A3F;">如果没有这个文件，请往下看    如果没有这个文件，请往下看</font>**

如果没有这个文件/不显示文件后缀，直接新建一个就行

我们先点击 “查看”- 显示“文件扩展名”



<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/63327424/1773628257819-98186c7c-3881-478b-9a52-70eb4cb74caf.png)

随后我们新建一个文本文档

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/63327424/1773628405384-1517a9fe-75ee-4c29-9400-37a717bf33e6.png)

将其更名为 .claude.json

##### 配置 <font style="background-color:#FBDE28;">settings.json</font>
**<font style="color:#DF2A3F;">如果没有settings.json文件，请自行创建</font>****<font style="color:rgb(52, 64, 84);">，不需要时可随意删除，不影响claude使用</font>**

`<font style="color:rgb(52, 64, 84);background-color:rgba(86, 87, 88, 0.04);">windows下路径为: C:/Users/你的用户名/.claude</font>`

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/png/63327424/1772855181489-8d2f5bb7-8f79-438a-a783-01baebbef2ff.png)

{

  "env": {

    "ANTHROPIC_AUTH_TOKEN": "<font style="color:#DF2A3F;">sk开头的 api key  这个就是我们注册兑换后，添加的令牌密钥，注意不要多空格</font>",

    "ANTHROPIC_BASE_URL": "[https://yunqiaoapi.com](https://yunqiaoapi.com)",

    "ANTHROPIC_MODEL": "claude-sonnet-4-6"

  },

  "includeCoAuthoredBy": false,

  "model": "Sonnet"

}



### <font style="color:rgb(31, 35, 40);">第六步：启动Claude</font>
打开 PowerShell，直接启动 Claude Code：

输入：claude

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/webp/63327424/1769487171264-d826aabd-2826-40bb-bff1-78b3b3fccc1b.webp)

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/webp/63327424/1769487178393-34b9c4f1-538d-40c0-9e5f-e3cb6e621ea2.webp)

<font style="color:rgb(138, 143, 141);">设置主题颜色</font>

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/webp/63327424/1769487188714-5f212010-1ef7-4a6d-b800-c12214e91a33.webp)

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/webp/63327424/1769487193534-43f01a2b-5050-454a-8e2f-d0333354af6b.webp)

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/webp/63327424/1769487193534-43f01a2b-5050-454a-8e2f-d0333354af6b.webp) 

<font style="color:rgb(138, 143, 141);">是否信赖该文件夹</font>

<font style="color:rgb(138, 143, 141);"></font>

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/webp/63327424/1769487201709-38fc0b86-c72d-40a4-975d-855a6052de46.webp?date=1776657578837)

输入：/model **按 Enter 进入，选择模型，通常使用默认设置即可。**

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/webp/63327424/1769487270437-5c80b5b1-5333-4c59-851a-fe37a5a80426.webp)

<!-- 这是一张图片，ocr 内容为： -->
![](https://cdn.nlark.com/yuque/0/2026/webp/63327424/1769487277874-c1156e5e-15e5-4c74-9dc0-eaca0ddac36b.webp)

到此为止就算Claude Code安装完成

_**<font style="color:rgb(10, 10, 10);">注意：设置环境变量修改后，使用所有模型（包括官方预设模型）均调用自定义接入点，而不使用官方账号额度。</font>**_

