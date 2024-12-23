<div align="center">
  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
  <br>
  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
</div>

<div align="center">

# none-plugin-OI-helper

_✨ NoneBot 插件简单描述 ✨_

<a href="./LICENSE">
    <img src="https://img.shields.io/github/license/talentestors/none-plugin-oi-helper.svg" alt="license">
</a>
<a href="https://pypi.python.org/pypi/none-plugin-oi-helper">
    <img src="https://img.shields.io/pypi/v/none-plugin-oi-helper.svg" alt="pypi">
</a>
<img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">

</div>

## 📖 介绍

一个基于 <https://clist.by> v4 接口的查询比赛信息的接口插件。

扩展内容：

- [x] 获取 **LeetCode 每日一题**
- [x] 获取 **洛谷日报**
- [ ] ...

## 💿 安装

<details>
<summary>使用 nb-cli 安装</summary>

在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装

```bash
nb plugin install nonebot-plugin-oi-help # 未上架商店
```

</details>

<details>
<summary>使用包管理器安装</summary>

在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令

<details>
<summary>pip</summary>

```bash
pip install nonebot-plugin-oi-help
```

</details>

<details>
<summary>pdm</summary>

```bash
pdm add nonebot-plugin-oi-help
```

</details>

<details>
<summary>poetry</summary>

```bash
poetry add nonebot-plugin-oi-help
```

</details>

<details>
<summary>conda</summary>

```bash
conda install nonebot-plugin-oi-help
```

</details>

<details>
<summary>uv</summary>

[uv:](https://github.com/astral-sh/uv) <https://docs.astral.sh/uv/>

```bash
uv add nonebot-plugin-oi-help
```

</details>

打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入

```bash
plugins = ["nonebot-plugin-oi-help"]
```

</details>

## ⚙️ 配置

在 nonebot2 项目的`.env`文件中添加下表中的必填配置

> [!TIP]
> 需要使用 aiohttp 的驱动器

| 配置项 | 必填 | 默认值 | 说明 |
|:-----:|:----:|:----:|:----:|
| CLIST__USERNAME | 是 | 无 | 你的clist用户名 |
| CLIST__USER_KEY | 是 | 无 | 你的 key |
| CLIST_API__REQ_URL | 否 | <https://clist.by:443/api/v4/contest/?upcoming=true&filtered=true&order_by=start&format=json> | 自定义查询url |

### 如何获取 clist 的 key？

1. 进入CLIST官网：<https://clist.by/>
2. 如果你是新用户，你需要新建一账户。
3. 前往 <https://clist.by/api/v4/doc/> 页面
    - 也可以去这里进去：
    ![api](docs/img/image.png)
4. 点 here 获取你的 API KEY
    - > Accessing the API requires an API key, available to authenticated users _here_.

    ![here](docs/img/guide.png)

## 🎉 使用

[see docs](./docs/README.md)
