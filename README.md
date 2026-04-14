# HappyHorse AI GitHub Pages

这是一个基于 **GitHub Pages + Jekyll** 的独立导航/SEO 站点，用于覆盖以下搜索意图：

- `HappyHorse AI`
- `Happy Horse`
- `HappyHorse API`
- `AI Video Generator`
- `HappyHorse GitHub`

站点定位不是“官方品牌站”，而是**独立信息导航站**。当前对外体验入口采用 `https://www.happy-horse.net`，但仓库中的文案不会把它写死为“官方归属已验证”。

## 当前结构

- `index.md`: 首页总入口
- `happyhorse-ai.md`: 核心品牌词落地页
- `happyhorse-api.md`: API 搜索意图页
- `happyhorse-github.md`: GitHub 搜索意图页
- `ai-video-generator.md`: 泛词页
- `official-site.md`: “official site” 搜索词页
- `faq.md`: FAQ 页
- `_layouts/default.html`: 全站布局
- `assets/css/style.scss`: 主题样式覆盖
- `.github/workflows/pages.yml`: GitHub Pages 自动部署工作流

## 发布方式

推荐使用 **GitHub Actions**，因为这是 GitHub 文档现在推荐的方式。

1. 把仓库推送到默认分支 `main`
2. 打开仓库 `Settings -> Pages`
3. 在 `Build and deployment` 中选择 `GitHub Actions`
4. 等待 `.github/workflows/pages.yml` 运行完成

发布成功后，用户站点地址应为：

- `https://happyhorse-ai-video.github.io/`

## 本地预览

如果本机有 Ruby 环境，可以用下面的方式本地预览：

1. `bundle install`
2. `bundle exec jekyll serve`
3. 打开 `http://127.0.0.1:4000/`

如果系统自带 Ruby 过旧而导致 `bundle install` 失败，优先用 GitHub Actions 作为构建入口，或者升级到较新的 Ruby 版本后再本地预览。

## 后续建议

1. 补对比页，例如 `HappyHorse vs Kling`、`HappyHorse vs Seedance`
2. 新增更新页或 changelog，承接版本相关搜索
3. 一旦拿到可验证的 API 文档、官方仓库、官方站点，再把对应页面升级为强信息页
4. 如果仓库所属账号或域名变化，记得同步更新 `_config.yml` 里的 `url`
