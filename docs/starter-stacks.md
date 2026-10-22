# 按场景搭配工具

这些组合用于说明不同服务如何分工。先选择当前需要的能力，费用与条款参阅[费用说明](pricing-notes.md)和对应官网。

## 个人官网、博客、产品介绍页

| 需求 | 可选方案 | 什么时候加入 |
| --- | --- | --- |
| 域名 | Spaceship 或 Porkbun | 需要独立品牌地址时。 |
| DNS | Cloudflare 或 DNSPod | 将域名接到网站部署平台时。 |
| 部署 | Cloudflare Workers / Pages 或 Netlify | 首次上线时，先确认构建和运行时支持。 |
| 内容 | Markdown；需要编辑后台时比较 Keystatic | 文章和内容开始持续更新时。 |
| 统计 | Umami、Plausible 或 Google Analytics，先选一种 | 需要知道访问来源和热门页面时。 |
| 搜索表现 | Google Search Console 和 Bing Webmaster Tools | 网站公开且希望获取搜索流量时。 |
| 联系入口 | 域名邮箱或邮件转发；需要表单时加入 Tally | 希望用户联系或提交反馈时。 |

纯内容网站通常可以先用静态文件，无需为工具目录提前配置数据库或用户系统。

## 带登录和用户数据的 Web 工具

| 需求 | 可选方案 | 如何取舍 |
| --- | --- | --- |
| 网站与 API 部署 | Cloudflare Workers、Netlify 或适合用途的 Vercel 套餐 | 先检查框架、Node.js 依赖和运行时支持。 |
| 数据库 | Supabase 或 Neon | 需要数据库与配套后端能力时比较 Supabase；PostgreSQL 为主时也可以比较 Neon。 |
| 登录 | Supabase Auth、Clerk 或 Better Auth | 按已有后端、预制界面需求和自行维护能力选择一个主方案。 |
| 用户文件 | Supabase Storage 或 Cloudflare R2 | 有图片、附件等上传需求时再加入。 |
| 系统邮件 | Resend 或 Postmark | 注册验证、密码重置和产品通知需要邮件时接入，并检查认证平台已有能力。 |
| 业务分析 | PostHog、Mixpanel 或 OpenPanel | 明确关键操作后，再设计注册和使用漏斗。 |
| 错误追踪 | Sentry 或 GlitchTip | 开始接收真实用户流量时，建立报错排查入口。 |
| 在线监控 | UptimeRobot 或自部署的 Uptime Kuma | 服务需要持续可用并在中断时告警。 |

数据库、认证和文件权限需要一起设计；采用同一平台可以减少集成环节，但仍需配置业务权限。

## 内容站、导航站、工具合集

| 需求 | 可选方案 | 如何取舍 |
| --- | --- | --- |
| 内容数据 | Markdown 或结构化文件 | 条目由开发者维护时，先随代码管理。 |
| 内容编辑 | Keystatic 或 Sanity | 非开发者需要持续维护内容时，再引入编辑界面。 |
| 站内搜索 | 本地搜索；内容规模扩大后比较 Algolia、Meilisearch 或 Typesense | 先依据条目量、筛选需求和更新频率决定。 |
| 搜索收录 | Google Search Console、Bing Webmaster Tools | 检查站点地图、抓取和搜索表现。 |
| SEO 排查 | PageSpeed Insights、Screaming Frog、Rich Results Test | 分别检查性能、页面结构和结构化数据。 |
| 选题研究 | Google Trends；深入研究时比较 Ahrefs 或 Semrush | 先验证兴趣趋势，再评估是否需要付费研究工具。 |

对于 OPCHub，第一步可以直接维护 GitHub README；需要分类筛选和搜索时，再将相同内容组织成网站。

## 接入顺序

1. 先完成部署、域名和关键功能。
2. 再补错误追踪、在线监控和必要的联系渠道。
3. 有真实访问后，围绕具体问题加入统计、回放和 SEO 工具。
4. 需要多人维护或内容规模变大时，再增加 CMS、独立搜索等服务。
