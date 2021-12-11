1. 安装插件
    # 1. 安装 PSReadline 包，该插件可以让命令行很好用，类似 zsh
    Install-Module -Name PSReadLine

    # 2. 安装 posh-git 包，让你的 git 更好用
    Install-Module posh-git

    # 3. 安装 oh-my-posh 包，让你的命令行更酷炫、优雅,注意，新版的
    # oh-my-posh 可能会使中文提示信息乱码。所以安装时可以指定以前
    # 版本。
    #Install-Module oh-my-posh
    Install-Module oh-my-posh -RequiredVersion 3.112.1
    
    Install-Module DirColors
    Install-Module git-aliases
    
2. 配置 powershell
    在 power shell 中输入如下命令
    vim $PROFILE
    输入"Microsoft.PowerShell_profile.ps1"文件中的内容

    > 参考网址：https://zhuanlan.zhihu.com/p/137595941

3. 配置 oh-my-posh 主题

   * 在命令行中查看所有的主题：Get-PoshThemes

   * 在"Microsoft.PowerShell_profile.ps1"中配置主题比如：

     #设置 PowerShell 主题                                                                                      

     Set-PoshPrompt -Theme robbyrussel 
