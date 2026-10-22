# 出海独立开发免费套件

[返回工具总目录](../README.md) · [查看费用说明](pricing-notes.md) · [查看场景搭配](starter-stacks.md)

这张表参考用户提供的 Corey Chiu（@realcoreychiu）「出海独立开发免费套件」截图整理，图中文字标注为「2025 最新」。保留图中的工具组合与排列顺序，并补充每一类解决的问题和官方资料。

「免费套件」沿用参考图名称：其中包含免费版、免费额度、开源自部署、免费试用和付费项目，不能将整套理解为零成本。按本项目的收录范围，原图中的支付项未纳入本表。

## 套件一览

费用说明整理于 **2026-10-22**。所链接的官方资料用于补充参考图，不代表逐项注册或实测；本轮无法完整读取的套餐信息已标注待核验。

| 类别 | 参考图中的工具组合 | 解决什么问题 | 费用与使用说明 |
| --- | --- | --- | --- |
| 域名购买 | [Spaceship](https://www.spaceship.com/domains/) / [Sav](https://sav.com/) / [Regery](https://regery.com/) | 购买和管理网站域名，例如 `your-product.com`。 | 域名通常需要付费注册和续费；同时比较首年价格、续费价与转移条件。原图这一项没有标注免费。 |
| 域名解析 | [Cloudflare DNS](https://developers.cloudflare.com/dns/) | 将域名连接到部署平台，配置网站和邮箱所需的 DNS 记录。 | DNS、代理/CDN 与其他 Cloudflare 产品分别有功能和套餐范围，按实际使用能力核对[官方方案](https://www.cloudflare.com/plans/)。 |
| 数据库 | [Supabase](https://supabase.com/) | 保存用户、业务记录及产品内容，配套 API、认证和存储能力。 | 有免费额度；注意项目数量、容量、流量、闲置暂停和备份差异。[官方定价](https://supabase.com/pricing) |
| Auth | [Supabase Auth](https://supabase.com/auth) / [Clerk](https://clerk.com/) | 实现注册、登录、身份验证和用户管理。 | 都有免费方案或额度；用户计量口径与高级认证功能要分别查看。[Supabase 定价](https://supabase.com/pricing) / [Clerk 定价](https://clerk.com/pricing) |
| 缓存 | [Upstash Redis](https://upstash.com/) | 缓存数据，支持计数、接口限流等用途。 | 提供免费及付费方案，请核对请求量、存储和吞吐限制。[官方定价](https://upstash.com/pricing/redis) |
| 存储 | [Cloudflare R2](https://developers.cloudflare.com/r2/) | 保存图片、附件、音视频及下载文件。 | 提供免费额度；存储、操作次数和存储类别有独立规则，免出站流量费不等于无限免费。[官方定价](https://developers.cloudflare.com/r2/pricing/) |
| 部署 | [Vercel](https://vercel.com/) / [Cloudflare Pages](https://developers.cloudflare.com/pages/) | 将代码构建并发布成可访问的网站。 | Vercel Hobby 限个人、非商业用途；Cloudflare 也需区分静态部署、Functions / Workers 等能力的限制。[Vercel 条款](https://vercel.com/docs/plans/hobby) / [Cloudflare 平台定价](https://www.cloudflare.com/plans/developer-platform/) |
| 域名邮件 | [Resend](https://resend.com/) ＋ [Cloudflare Email Routing](https://developers.cloudflare.com/email-service/) | 使用 Resend 发送验证码、通知；将域名来信转到已有邮箱。 | Resend 免费方案有发送限制；转发、发信、日常邮箱是不同能力。Cloudflare 路由与 Beta 发信能力分别配置。[Resend 定价](https://resend.com/pricing) / [Cloudflare 文档](https://developers.cloudflare.com/email-service/) |
| 统计 | [Google Analytics](https://marketingplatform.google.com/about/analytics/) / [OpenPanel](https://openpanel.dev/) / [PostHog](https://posthog.com/) | 了解访客来源、访问页面、产品事件和转化路径。 | 不应统一标成免费：GA 可从标准版了解起；PostHog 各产品有免费额度；OpenPanel 云服务目前提供免费试用，自部署另计运行成本。[GA](https://marketingplatform.google.com/about/analytics/) / [PostHog 定价](https://posthog.com/pricing) / [OpenPanel](https://openpanel.dev/) |
| 监控 | [Sentry](https://sentry.io/) | 收集应用错误及上下文，帮助定位用户遇到的异常。 | 有免费 Developer 方案，事件额度与成员数有限；它侧重应用错误追踪，网站可用性监控可按需求另配。[官方方案说明](https://www.sentry.help/en/articles/13965074-what-happens-if-i-cancel-my-plan) |
| CMS | [Sanity](https://www.sanity.io/) / [Keystatic](https://keystatic.com/) | 管理文章、产品说明和网站内容。 | Sanity 有 Free 方案；Keystatic 可管理本地或 Git 中的内容文件，云服务与运行环境另看条件。[Sanity 定价](https://www.sanity.io/pricing) / [Keystatic 文档](https://keystatic.com/docs) |
| 设计 | [Figma](https://www.figma.com/) | 绘制页面、交互原型和设计规范。 | 提供免费 Starter 方案，产品功能和协作范围有限。[官方定价](https://www.figma.com/pricing/) |
| 代码编辑器 | [Windsurf](https://windsurf.com/) | 在编辑器中编写、理解和修改代码。 | 图中写「10 刀/月」，属于旧图信息；本轮查阅时原定价入口重定向至 Devin 定价页，不沿用旧月费。[当前定价入口](https://windsurf.com/pricing) |
| AI 辅助 | [ChatGPT](https://chatgpt.com/) | 辅助梳理需求、解释代码、撰写文案和排查问题。 | 图中列为免费；本轮未完整读取官方套餐内容，免费功能及用量待核验，不记录固定模型或额度。[官方套餐入口](https://chatgpt.com/pricing/) |
| 笔记 | [Obsidian](https://obsidian.md/) / [Notion](https://www.notion.com/) / [飞书](https://www.feishu.cn/) | 记录想法、需求、调研和项目知识。 | Obsidian 基础应用免费，Sync / Publish 等附加服务付费；Notion 有 Free 方案；飞书当前套餐详情本轮未完整读取，待核验。[Obsidian 定价](https://obsidian.md/pricing) / [Notion 定价](https://www.notion.com/pricing) / [飞书版本对比](https://www.feishu.cn/service) |
| 代码管理 | [GitHub](https://github.com/) | 保存代码历史，管理 Issue、Pull Request 和项目协作。 | 提供 Free 及付费套餐；Actions、存储和其他附加服务有独立用量规则。[官方定价](https://github.com/pricing) |
| 任务管理 | [Notion](https://www.notion.com/) / [飞书](https://www.feishu.cn/) | 通过文档、看板和表格组织开发任务与项目进度。 | Notion 的 Free 与团队套餐有差异；飞书当前套餐待核验，使用前核对人数、存储及高级功能。[Notion 定价](https://www.notion.com/pricing) / [飞书版本对比](https://www.feishu.cn/service) |
| SEO | [Google Trends](https://trends.google.com/) / [Ahrefs](https://ahrefs.com/) / [Semrush](https://www.semrush.com/) | 研究搜索兴趣、关键词、竞争网站和外链。 | Trends 反映相对兴趣趋势；Ahrefs 免费功能有范围限制，完整研究功能与 Semrush 付费产品分别选型。[Ahrefs 免费功能](https://help.ahrefs.com/en/articles/13002606-what-can-i-use-for-free-in-ahrefs) / [Semrush 定价](https://www.semrush.com/pricing/) |

## 如何读这套组合

- **基础运行**：域名 → DNS → 部署，先让网站可以访问。
- **业务功能**：数据库、认证、缓存和存储按产品需要加入，不必一次全部接入。
- **用户沟通**：Resend 与邮件转发分别负责应用发信和接收域名来信。
- **持续改进**：统计帮助理解使用情况，Sentry 帮助定位异常，SEO 工具帮助研究搜索需求。
- **开发协作**：设计、编辑器、AI、笔记和任务管理服务于日常开发，按已有习惯选用。

同一类别中的 `/` 表示备选工具，不表示必须同时购买或使用。Resend 与邮件转发的 `＋` 表示两种不同用途的组合。

## 来源与维护

参考来源为用户提供的署名截图；未提供原帖链接，因此不补写或推测原帖地址。此文是基于截图的用途整理与官方资料补充，未转载截图图片，也不代表原作者对本项目的背书。

更新价格或免费条件时，请同步记录官方来源和核验日期。更细的费用区别见[费用说明](pricing-notes.md)，完整同类工具见[总目录](../README.md)。
