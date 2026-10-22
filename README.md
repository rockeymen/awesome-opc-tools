# OPCHub · 独立开发者工具指南

为一人公司（OPC）和独立开发者整理的工具与服务合集，覆盖从产品开发、网站上线到数据分析和用户增长的常见需求。

每个工具都说明「解决什么问题」和「适合什么场景」，帮助你按需求选型。收录范围包含商业服务、开源软件和本地开发工具。

## 导航

- [基础设施](#基础设施)：域名、DNS、部署、服务器、数据库、缓存、存储、媒体处理、搜索。
- [产品开发](#产品开发)：认证、AI 编程、代码托管、设计、组件、接口调试、测试、CMS、文档。
- [邮件与用户沟通](#邮件与用户沟通)：域名邮箱、邮件转发、系统邮件、营销邮件、表单、客服。
- [数据分析与增长](#数据分析与增长)：流量统计、事件埋点、行为回放、监控、SEO、产品发布。
- [按场景搭配工具](docs/starter-stacks.md)
- [免费方案与费用说明](docs/pricing-notes.md)
- [贡献指南](CONTRIBUTING.md)

## 如何使用这份指南

1. 根据当前遇到的问题找分类，不必一次接入所有服务。
2. 对比同类工具的技术栈、部署方式和维护成本，再决定采用哪一种。
3. 查看官方定价和使用限制。有免费额度、免费试用、开源自部署，是三种不同情况。

下表是用途目录，不代表所有工具都免费、开源或经过项目实测。费用核验范围与日期单独记录在[费用说明](docs/pricing-notes.md)中。国内访问体验、注册条件和支付方式需要按实际使用环境确认。

## 基础设施

<table>
  <thead>
    <tr><th>分类</th><th>工具</th><th>介绍与适用场景</th></tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="3" align="center" valign="middle">域名注册</td>
      <td><a href="https://www.spaceship.com/domains/">Spaceship</a></td>
      <td>购买、续费和转移域名；选购时同时比较首年价与续费价。</td>
    </tr>
    <tr>
      <td><a href="https://porkbun.com/">Porkbun</a></td>
      <td>域名注册与管理服务，可作为购买域名时的比价选项。</td>
    </tr>
    <tr>
      <td><a href="https://www.namecheap.com/">Namecheap</a></td>
      <td>提供域名注册及配套服务，适合集中管理多个项目的域名。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">DNS 与 CDN</td>
      <td><a href="https://www.cloudflare.com/">Cloudflare</a></td>
      <td>集成域名解析、CDN 和网站防护，适合管理网站的访问入口。</td>
    </tr>
    <tr>
      <td><a href="https://www.dnspod.cn/">DNSPod</a></td>
      <td>域名解析和记录管理服务，可作为面向国内用户的解析方案之一。</td>
    </tr>
    <tr>
      <td rowspan="3" align="center" valign="middle">网站部署</td>
      <td><a href="https://developers.cloudflare.com/workers/">Cloudflare Workers / Pages</a></td>
      <td>部署网站、静态资源和边缘接口，适合工具站、内容站及轻量应用；根据运行时选择具体产品。</td>
    </tr>
    <tr>
      <td><a href="https://vercel.com/">Vercel</a></td>
      <td>提供前端应用部署和预览环境，适合 Next.js 等项目；Hobby 套餐有用途限制。</td>
    </tr>
    <tr>
      <td><a href="https://www.netlify.com/">Netlify</a></td>
      <td>连接代码仓库部署网站，提供预览部署和 Functions 等能力，适合静态网站及 Web 应用。</td>
    </tr>
    <tr>
      <td rowspan="3" align="center" valign="middle">云服务器</td>
      <td><a href="https://www.hetzner.com/cloud/">Hetzner Cloud</a></td>
      <td>提供云服务器，适合自行运行后端、Docker 服务及常驻进程；需要承担运维。</td>
    </tr>
    <tr>
      <td><a href="https://www.aliyun.com/">阿里云</a></td>
      <td>提供服务器、数据库、存储等云产品，适合需要国内云资源和配套服务的项目。</td>
    </tr>
    <tr>
      <td><a href="https://cloud.tencent.com/">腾讯云</a></td>
      <td>提供服务器与云开发等产品，可按自建后端或托管开发需求选型。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">应用托管</td>
      <td><a href="https://railway.com/">Railway</a></td>
      <td>从代码或容器部署应用，并管理关联服务，适合希望减少服务器配置工作的后端项目。</td>
    </tr>
    <tr>
      <td><a href="https://render.com/">Render</a></td>
      <td>托管 Web 服务、静态网站和后台任务，适合将应用部署交给平台管理。</td>
    </tr>
    <tr>
      <td rowspan="4" align="center" valign="middle">数据库与后端</td>
      <td><a href="https://supabase.com/">Supabase</a></td>
      <td>以 PostgreSQL 为核心，配套认证、存储和 API，适合快速搭建带用户系统的产品。</td>
    </tr>
    <tr>
      <td><a href="https://neon.com/">Neon</a></td>
      <td>提供托管 PostgreSQL 及数据库分支等能力，适合需要关系数据库和开发环境隔离的应用。</td>
    </tr>
    <tr>
      <td><a href="https://firebase.google.com/">Firebase</a></td>
      <td>提供数据库、认证等应用后端能力，适合 Web 与移动应用集成。</td>
    </tr>
    <tr>
      <td><a href="https://developers.cloudflare.com/d1/">Cloudflare D1</a></td>
      <td>基于 SQLite SQL 语义的托管数据库，适合与 Workers 组合构建轻量业务接口。</td>
    </tr>
    <tr>
      <td align="center" valign="middle">缓存与限流</td>
      <td><a href="https://upstash.com/">Upstash Redis</a></td>
      <td>提供托管 Redis，适合缓存、计数、限流及 Serverless 应用的数据访问。</td>
    </tr>
    <tr>
      <td align="center" valign="middle">消息队列</td>
      <td><a href="https://developers.cloudflare.com/queues/">Cloudflare Queues</a></td>
      <td>在服务之间异步传递消息，适合将耗时任务从用户请求中拆出。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">对象存储</td>
      <td><a href="https://developers.cloudflare.com/r2/">Cloudflare R2</a></td>
      <td>保存图片、附件和下载资源；存储量、操作次数与出站流量采用不同计费规则。</td>
    </tr>
    <tr>
      <td><a href="https://aws.amazon.com/s3/">Amazon S3</a></td>
      <td>通用对象存储服务，适合文件保存、备份和与 AWS 服务配合使用。</td>
    </tr>
    <tr>
      <td rowspan="3" align="center" valign="middle">图片与视频</td>
      <td><a href="https://cloudinary.com/">Cloudinary</a></td>
      <td>提供媒体上传、转换和分发，适合需要动态生成多种图片尺寸的网站。</td>
    </tr>
    <tr>
      <td><a href="https://imagekit.io/">ImageKit</a></td>
      <td>提供媒体优化、转换和交付，适合图片较多的产品页、图库和内容站。</td>
    </tr>
    <tr>
      <td><a href="https://www.mux.com/">Mux</a></td>
      <td>提供视频处理、播放与相关分析能力，适合需要集成视频内容的产品。</td>
    </tr>
    <tr>
      <td rowspan="3" align="center" valign="middle">站内搜索</td>
      <td><a href="https://www.algolia.com/">Algolia</a></td>
      <td>托管搜索服务，适合产品目录、内容站和文档的搜索功能。</td>
    </tr>
    <tr>
      <td><a href="https://www.meilisearch.com/">Meilisearch</a></td>
      <td>提供全文搜索和检索能力，可比较托管与自部署方案，适合为已有内容增加搜索。</td>
    </tr>
    <tr>
      <td><a href="https://typesense.org/">Typesense</a></td>
      <td>提供即时搜索、筛选等能力，适合目录、商品和文档检索。</td>
    </tr>
  </tbody>
</table>

## 产品开发

<table>
  <thead>
    <tr><th>分类</th><th>工具</th><th>介绍与适用场景</th></tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="3" align="center" valign="middle">用户认证</td>
      <td><a href="https://clerk.com/">Clerk</a></td>
      <td>提供注册、登录、用户管理及预制界面，适合希望快速集成用户系统的应用。</td>
    </tr>
    <tr>
      <td><a href="https://supabase.com/auth">Supabase Auth</a></td>
      <td>与 Supabase 数据库和权限体系配合使用，适合已采用 Supabase 的产品。</td>
    </tr>
    <tr>
      <td><a href="https://better-auth.com/">Better Auth</a></td>
      <td>将认证逻辑集成到应用中的框架，适合希望控制认证流程及数据存储的开发者。</td>
    </tr>
    <tr>
      <td rowspan="4" align="center" valign="middle">AI 编程</td>
      <td><a href="https://cursor.com/">Cursor</a></td>
      <td>集成 AI 的代码编辑器，适合在编辑器中理解、生成和修改项目代码。</td>
    </tr>
    <tr>
      <td><a href="https://code.claude.com/">Claude Code</a></td>
      <td>面向项目代码的编程助手，适合通过自然语言执行开发和调试任务。</td>
    </tr>
    <tr>
      <td><a href="https://openai.com/codex/">Codex</a></td>
      <td>编程代理，适合围绕代码仓库完成实现、检查、修复和审查等任务。</td>
    </tr>
    <tr>
      <td><a href="https://github.com/features/copilot">GitHub Copilot</a></td>
      <td>提供代码补全、对话及编程辅助，适合与现有编辑器和 GitHub 工作流结合。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">代码托管</td>
      <td><a href="https://github.com/">GitHub</a></td>
      <td>托管代码、管理 Issue 和 Pull Request，适合开源协作和项目版本管理。</td>
    </tr>
    <tr>
      <td><a href="https://gitlab.com/">GitLab</a></td>
      <td>提供代码托管和开发协作能力，可按托管服务或自部署需求选型。</td>
    </tr>
    <tr>
      <td align="center" valign="middle">自动构建</td>
      <td><a href="https://github.com/features/actions">GitHub Actions</a></td>
      <td>在代码变更后执行构建、测试和发布流程，适合将重复开发步骤自动化。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">UI 设计</td>
      <td><a href="https://www.figma.com/">Figma</a></td>
      <td>界面设计、交互原型和设计协作工具，适合在编码前确定产品结构。</td>
    </tr>
    <tr>
      <td><a href="https://penpot.app/">Penpot</a></td>
      <td>开源设计与原型平台，适合关注开放格式、协作及自部署的团队。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">组件库</td>
      <td><a href="https://ui.shadcn.com/">shadcn/ui</a></td>
      <td>将可修改的组件代码加入项目，适合需要自行控制 React 界面细节的应用。</td>
    </tr>
    <tr>
      <td><a href="https://daisyui.com/">DaisyUI</a></td>
      <td>基于 Tailwind CSS 的组件库，适合快速构建常见表单、导航和页面布局。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">图标</td>
      <td><a href="https://lucide.dev/">Lucide</a></td>
      <td>风格统一的图标库，适合产品界面的按钮、菜单和状态提示。</td>
    </tr>
    <tr>
      <td><a href="https://iconify.design/">Iconify</a></td>
      <td>汇集多个图标集及使用工具，适合搜索和集成不同风格的图标。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">API 调试</td>
      <td><a href="https://www.usebruno.com/">Bruno</a></td>
      <td>本地 API 客户端，可将请求集合随代码版本管理，适合开发和复现接口请求。</td>
    </tr>
    <tr>
      <td><a href="https://hoppscotch.io/">Hoppscotch</a></td>
      <td>API 请求与调试工具，适合快速检查接口参数、鉴权和返回内容。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">自动化测试</td>
      <td><a href="https://playwright.dev/">Playwright</a></td>
      <td>驱动真实浏览器执行测试，适合验证登录、表单和关键页面交互。</td>
    </tr>
    <tr>
      <td><a href="https://vitest.dev/">Vitest</a></td>
      <td>JavaScript / TypeScript 测试框架，适合验证业务函数和组件逻辑。</td>
    </tr>
    <tr>
      <td rowspan="3" align="center" valign="middle">内容管理</td>
      <td><a href="https://www.sanity.io/">Sanity</a></td>
      <td>结构化内容管理平台，适合管理网站文章、页面及可复用内容。</td>
    </tr>
    <tr>
      <td><a href="https://keystatic.com/">Keystatic</a></td>
      <td>为 Markdown、YAML 等文件提供内容编辑界面，适合内容随 Git 仓库维护的网站。</td>
    </tr>
    <tr>
      <td><a href="https://strapi.io/">Strapi</a></td>
      <td>Headless CMS，适合自行定义内容模型，并通过 API 向网站或 App 提供内容。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">产品文档</td>
      <td><a href="https://vitepress.dev/">VitePress</a></td>
      <td>将 Markdown 构建成文档网站，适合工具说明、开发文档和知识库。</td>
    </tr>
    <tr>
      <td><a href="https://docusaurus.io/">Docusaurus</a></td>
      <td>基于 React 的文档网站工具，适合需要文档版本和多语言组织的项目。</td>
    </tr>
  </tbody>
</table>

## 邮件与用户沟通

<table>
  <thead>
    <tr><th>分类</th><th>工具</th><th>介绍与适用场景</th></tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2" align="center" valign="middle">域名邮箱</td>
      <td><a href="https://www.zoho.com/mail/">Zoho Mail</a></td>
      <td>提供企业邮箱托管，适合使用自己的域名日常收发邮件。</td>
    </tr>
    <tr>
      <td><a href="https://workspace.google.com/">Google Workspace</a></td>
      <td>提供企业邮箱及办公协作套件，适合统一管理邮箱、日历和文档。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">邮件转发</td>
      <td><a href="https://developers.cloudflare.com/email-service/">Cloudflare Email Routing</a></td>
      <td>将域名地址收到的邮件转到已有邮箱；官网现归入 Email Service，路由与发信需分开配置。</td>
    </tr>
    <tr>
      <td><a href="https://improvmx.com/">ImprovMX</a></td>
      <td>提供域名邮件别名和转发，适合集中接收多个公开联系地址的来信。</td>
    </tr>
    <tr>
      <td rowspan="3" align="center" valign="middle">系统邮件</td>
      <td><a href="https://resend.com/">Resend</a></td>
      <td>面向开发者的邮件 API，适合验证码、密码重置和产品通知。</td>
    </tr>
    <tr>
      <td><a href="https://postmarkapp.com/">Postmark</a></td>
      <td>提供事务邮件发送与投递相关工具，适合应用触发的通知邮件。</td>
    </tr>
    <tr>
      <td><a href="https://aws.amazon.com/ses/">Amazon SES</a></td>
      <td>云邮件发送服务，适合通过 API 或 SMTP 集成到已有后端。</td>
    </tr>
    <tr>
      <td rowspan="3" align="center" valign="middle">营销邮件</td>
      <td><a href="https://www.brevo.com/">Brevo</a></td>
      <td>邮件营销与自动化平台，适合用户分组、活动邮件和用户召回。</td>
    </tr>
    <tr>
      <td><a href="https://www.mailerlite.com/">MailerLite</a></td>
      <td>提供邮件通讯、订阅表单和自动化，适合维护 Newsletter 和订阅用户。</td>
    </tr>
    <tr>
      <td><a href="https://listmonk.app/">listmonk</a></td>
      <td>可自部署的订阅用户与邮件活动管理工具；实际发送还需要配置邮件通道。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">表单与反馈</td>
      <td><a href="https://tally.so/">Tally</a></td>
      <td>在线表单工具，适合需求调查、报名、反馈和候补名单。</td>
    </tr>
    <tr>
      <td><a href="https://formbricks.com/">Formbricks</a></td>
      <td>用户调查与反馈工具，适合在网站或产品中收集体验反馈。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">在线客服</td>
      <td><a href="https://crisp.chat/">Crisp</a></td>
      <td>提供网站聊天及用户沟通工具，适合在产品页面设置客服入口。</td>
    </tr>
    <tr>
      <td><a href="https://www.chatwoot.com/">Chatwoot</a></td>
      <td>客服会话与帮助中心平台，可比较云服务和自部署方案。</td>
    </tr>
  </tbody>
</table>

邮箱选型先明确需求：**日常收发找域名邮箱，集中收信找转发，验证码找系统邮件，订阅通讯找营销邮件**。同一平台可能覆盖多种用途，但套餐、投递限制和配置要求需要分别确认。

## 数据分析与增长

<table>
  <thead>
    <tr><th>分类</th><th>工具</th><th>介绍与适用场景</th></tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="3" align="center" valign="middle">流量统计</td>
      <td><a href="https://marketingplatform.google.com/about/analytics/">Google Analytics</a></td>
      <td>查看访问来源、页面表现和转化数据，适合分析网站获客效果。</td>
    </tr>
    <tr>
      <td><a href="https://umami.is/">Umami</a></td>
      <td>网站与产品分析工具，可比较云服务和自部署方案，适合查看访问及事件数据。</td>
    </tr>
    <tr>
      <td><a href="https://plausible.io/">Plausible</a></td>
      <td>注重简洁和隐私的网站分析工具，适合主要关注来源、页面及目标转化的网站。</td>
    </tr>
    <tr>
      <td rowspan="3" align="center" valign="middle">事件埋点</td>
      <td><a href="https://posthog.com/">PostHog</a></td>
      <td>集成事件分析、漏斗、留存及回放等能力，适合分析用户在产品内完成了什么操作。</td>
    </tr>
    <tr>
      <td><a href="https://mixpanel.com/">Mixpanel</a></td>
      <td>产品行为分析平台，适合比较用户分组、关键操作和转化路径。</td>
    </tr>
    <tr>
      <td><a href="https://openpanel.dev/">OpenPanel</a></td>
      <td>结合网站与产品分析，适合访问统计、事件追踪和漏斗分析；云服务与自部署分别选型。</td>
    </tr>
    <tr>
      <td align="center" valign="middle">行为回放</td>
      <td><a href="https://clarity.microsoft.com/">Microsoft Clarity</a></td>
      <td>提供热力图和会话回放，适合观察用户点击、滚动及操作卡点。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">错误追踪</td>
      <td><a href="https://sentry.io/">Sentry</a></td>
      <td>收集应用异常及相关上下文，适合定位前端、后端和移动应用错误。</td>
    </tr>
    <tr>
      <td><a href="https://glitchtip.com/">GlitchTip</a></td>
      <td>提供错误追踪等能力，可比较托管和自部署方式，适合集中排查应用报错。</td>
    </tr>
    <tr>
      <td align="center" valign="middle">日志与监控</td>
      <td><a href="https://betterstack.com/">Better Stack</a></td>
      <td>提供日志、在线监控与告警相关服务，适合集中查看运行状态和故障信息。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">在线监控</td>
      <td><a href="https://uptimerobot.com/">UptimeRobot</a></td>
      <td>定期检查网站或接口是否可访问，适合接收服务中断告警。</td>
    </tr>
    <tr>
      <td><a href="https://uptime.kuma.pet/">Uptime Kuma</a></td>
      <td>可自部署的在线监控与状态页工具，适合自行管理监控数据。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">搜索收录</td>
      <td><a href="https://search.google.com/search-console/about">Google Search Console</a></td>
      <td>查看 Google 搜索曝光、点击、收录和抓取问题，适合站长持续检查自然搜索表现。</td>
    </tr>
    <tr>
      <td><a href="https://www.bing.com/webmasters/about">Bing Webmaster Tools</a></td>
      <td>管理网站在 Bing 搜索中的表现和站长配置，适合补充搜索渠道。</td>
    </tr>
    <tr>
      <td rowspan="3" align="center" valign="middle">关键词研究</td>
      <td><a href="https://trends.google.com/">Google Trends</a></td>
      <td>比较搜索兴趣随时间和地区的变化，适合初步验证选题趋势；不等同于精确搜索量。</td>
    </tr>
    <tr>
      <td><a href="https://ahrefs.com/">Ahrefs</a></td>
      <td>提供关键词、外链、竞品与站点审计等工具，适合系统开展 SEO 研究。</td>
    </tr>
    <tr>
      <td><a href="https://www.semrush.com/">Semrush</a></td>
      <td>提供关键词、竞品及网站分析工具，适合研究自然搜索与营销机会。</td>
    </tr>
    <tr>
      <td align="center" valign="middle">技术 SEO</td>
      <td><a href="https://www.screamingfrog.co.uk/seo-spider/">Screaming Frog SEO Spider</a></td>
      <td>抓取网站并检查页面与链接问题，适合排查标题、重定向、重复内容和站内结构。</td>
    </tr>
    <tr>
      <td align="center" valign="middle">页面性能</td>
      <td><a href="https://pagespeed.web.dev/">PageSpeed Insights</a></td>
      <td>分析网页性能并提供改进建议，适合检查移动端与桌面端页面体验。</td>
    </tr>
    <tr>
      <td align="center" valign="middle">结构化数据</td>
      <td><a href="https://search.google.com/test/rich-results">Rich Results Test</a></td>
      <td>检查页面对 Google 富媒体搜索结果的结构化数据支持，适合验证标记实现。</td>
    </tr>
    <tr>
      <td rowspan="2" align="center" valign="middle">产品发布</td>
      <td><a href="https://www.producthunt.com/">Product Hunt</a></td>
      <td>发布和发现新产品，适合准备产品介绍、展示素材并获取早期反馈。</td>
    </tr>
    <tr>
      <td><a href="https://news.ycombinator.com/show">Show HN</a></td>
      <td>在 Hacker News 展示可体验的作品，适合向技术社区介绍产品和交流实现。</td>
    </tr>
    <tr>
      <td align="center" valign="middle">开发者社区</td>
      <td><a href="https://www.indiehackers.com/">Indie Hackers</a></td>
      <td>独立开发者社区，适合交流产品实践、开发过程和用户反馈。</td>
    </tr>
  </tbody>
</table>

统计工具的职责可以重叠，按问题选择即可：

- **谁来了、从哪里来？** 看流量统计。
- **注册后做了什么、在哪一步流失？** 看事件埋点和漏斗。
- **为什么点不下去、哪里让人困惑？** 看热力图和会话回放。
- **网站有没有挂、程序有没有报错？** 看在线监控和错误追踪。
- **搜索引擎能否发现页面？** 看站长工具和技术 SEO。

## 一起完善

欢迎补充工具、修正链接、更新官方费用与限制，也欢迎提交有版本、日期和使用环境的真实体验。

新增条目请参考[贡献指南](CONTRIBUTING.md)。以解决具体问题为收录依据，介绍保持简洁，优先引用官方来源。

## 许可证

本仓库的原创目录与说明采用 [CC BY 4.0](LICENSE) 许可证。署名可使用「[OPCHub / rockeymen](https://github.com/rockeymen/awesome-opc-tools)」。收录工具及其商标、代码和文档遵循各自的许可与服务条款。
