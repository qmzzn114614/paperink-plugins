# PaperInk 插件市场索引

这是 [PaperInk](https://github.com/qmzzn114614/PaperInk) 平板阅读器的插件市场索引仓库。

App 内「插件 → 插件市场」会读取本仓库的 [`index.json`](./index.json) 并列出可安装插件。

## index.json 格式

```json
{
  "plugins": [
    {
      "id": "com.example.myplugin",
      "name": "插件名称",
      "description": "一句话说明这个插件能干什么",
      "version": "1.0.0",
      "author": "作者名",
      "minHostVersion": "0.4.0",
      "tags": ["书签"],
      "apkUrl": "https://github.com/你/你的仓库/releases/download/v1.0.0/plugin.apk",
      "homepage": "https://github.com/你/你的仓库"
    }
  ]
}
```

- `id`：插件唯一 ID（与插件 manifest 一致），必填
- `name` / `description` / `version` / `author`：展示信息
- `apkUrl`：安装包下载地址，App 会打开这个链接让用户下载
- `homepage`：项目主页（可选）

## 如何收录自己的插件

1. Fork 本仓库；
2. 在 `plugins/` 下新建你的插件目录（放 README 与 APK 的 Release 说明）；
3. 在 `index.json` 的 `plugins` 数组里追加一条记录；
4. 提 PR。

## 官方索引地址（App 内置）

- jsDelivr：`https://gcore.jsdelivr.net/gh/qmzzn114614/paperink-plugins@main/index.json`
- 反代 raw：`https://gh-proxy.com/https://raw.githubusercontent.com/qmzzn114614/paperink-plugins/main/index.json`

## 已有插件

| 插件 | 说明 | 版本 |
| --- | --- | --- |
| 测试画星书签 | 演示插件：顶部面板 + 画星识别书签 | 1.0.0 |