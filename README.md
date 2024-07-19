# LeviLamina Easier (Auto 自动打包)

**此仓库与 Mojang Studio 无关，本仓库只提供了非官方(Mojang Studio, LiteDev)构建的服务器打包，您使用本仓库进行构建说明您已经同意了 EULA 条款**

一个自动打包最新版本的 带有 LeviLamina 环境的 Git Action

我们只希望以最高效、最方便的方式对 LeviLamina 进行安装

## 如何食用?

首先以此仓库为模板在您的帐户下建立一个新仓库

然后打开 `Action` 页面

点击右侧的 `Pack LeviLamina`

打开 `Run workflow` 填入你需要的 LeviLamina 版本号(本 README 上的蓝色小标签中的数字)，以及按照个人需求填写其他内容

点击 `Run workflow` 后，一杯白开水的功夫你就可以去 `Release` 里找到期待中的 `ll_ll版本号_所需bds版本号.zip` 啦！

## `Run workflow` 页中选项解释

| 名称          | 解释                      | 默认值        |
| ------------- | ------------------------- | ------------- |
| `LL_VER`      | `LeviLamina` 所需安装版本 | 0.1.0         |
| `LSE`         | 是否安装 `LSE`            | false         |
| `RUNTIME`     | 是否包括`LeviLamina`所需的C++运行时| false|
| `SCRIPTS`     | 是否运行仓库目录下的 `user_scripts.bat`|false|

-----

## 工作原理

在 Git Action 的服务器上先安装 lip ，之后利用 Git Action 的服务器“网速快”的“特性”，用 lip 安装 LeviLamina 之类，安装完成后再将其文件压缩并扔在 Release 中

## 有啥用?

新版的 LeviLamina 安装手动安装不是很简单，这对腐竹有一定技术要求；用 lip 自动安装网络又不太好导致安装过程出现各种奇怪问题，所以有了这个仓库以减轻开服难度

