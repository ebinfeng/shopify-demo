# Shopify 实战系列课程源码仓库

本仓库收录了「Shopify 实战系列开发课程」的配套源码。按照课程进度，不同章节或阶段会以 `course-序号` 的方式存放在独立目录中（例如：`course-001`、`course-002`）。每个目录代表一个可独立运行与学习的主题版本，便于对照课程内容进行实操与对比。

## 仓库结构

- `course-001/`：课程第 1 个阶段（或章节）的主题代码
- `course-002/`：课程第 2 个阶段（或章节）的主题代码

各 `course-*` 目录均为标准的 Shopify Online Store 2.0 主题结构，典型包含：

- `assets/`：静态资源（CSS、JS、图片等）
- `blocks/`：可复用区块（Block）定义
- `config/`：主题配置（如 `settings_schema.json`、`settings_data.json`）
- `layout/`：布局文件（例如 `theme.liquid`）
- `locales/`：多语言文案
- `sections/`：页面分区（Online Store 2.0 的核心）
- `snippets/`：可复用 Liquid 片段
- `templates/`：页面模板（如 `product.json`, `collection.json` 等）
- `.shopify/`：Shopify CLI 连接与环境配置
- `.theme-check.yml`：主题静态检查配置
- `.shopifyignore`：主题推送/预览时的忽略规则

## 环境准备

在开始之前，请确保：

- 已安装并登录 Shopify CLI（需要开发商店权限）
- 本地已安装 Node.js（部分工作流和工具可能依赖）

参考：Shopify CLI 文档（可从 Shopify 官方文档站点获取）

## 本地开发与预览

以下命令均需在具体的 `course-*` 目录下运行（以 `course-001` 为例）：

```bash
cd course-001
# 启动本地开发预览（首次会引导登录并连接开发商店）
shopify theme dev

# 进行主题静态检查
shopify theme check

# 将主题推送到商店（谨慎操作）
shopify theme push
```

需要切换到其它章节进行学习时，只需进入相应的 `course-xxx` 目录并重复上述流程。

## 学习建议

- 建议按照课程顺序逐一进入对应的 `course-*` 目录进行练习。
- 使用 `shopify theme check` 及时发现并修正 Liquid、Schema 等规范问题。
- 若想对比差异，可使用 Git 或 Diff 工具对不同 `course-*` 目录进行文件级比较，了解每个阶段的变更点。

## 贡献与反馈

- 欢迎在课程学习过程中提交 Issue 反馈问题或建议。
- 如需 PR，请遵循各 `course-*` 目录中的 `CONTRIBUTING.md` 及代码风格约定。

## 许可协议

本仓库中各 `course-*` 目录包含的主题示例代码遵循其各自目录内声明的许可证（通常为 `LICENSE.md`）。请在使用或分发前阅读相应文件。

