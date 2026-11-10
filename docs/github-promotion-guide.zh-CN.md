# GitHub 公开文档发布与引流指引

这份 README 用英文生日福利领取指南承接读者需求，通过有用的检查表、分类导航和品牌条件说明，引导有需要的人访问网站。GitHub 的作用是公开展示、品牌发现、推荐访问和获得真实引用；不能把一次发布等同于“增加权重”或排名提升。

## 本次采用的方法与来源边界

- 哥飞方法论依据：本地网站源码中的 `docs/seo-growth-plan.md` 第 1 章及来源说明。该文件注明摘录自“哥飞公众号文章同步”知识库、《养网站防老》等文章。本次没有直接访问原知识库，因此这里是依据项目已有摘录做的应用设计，不是对原文或其最新观点的独立核验。
- 按搜索意图组织内容：围绕生日福利怎么找、何时注册、是否需要消费、如何兑换等真实问题写指南，以列表导航连接网站首页、分类页和品牌页。
- 提供信息增益：增加可复制领取检查表；区分免费、消费条件、待核实和参考记录；解释邮件优惠与实物邮寄的差别。
- 避免照搬旧计划：旧计划中的品牌数量和路线状态已经过时。内容与路由以当前源码及 2026-11-10 的线上检查为准，不宣传未上线的 guides、kids 或 near-me 页面，也不拿缺乏本地参与证据的地区页做推广落点。
- GitHub README 展示和 topics 配置依据 [GitHub README 文档](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)及 [topics 文档](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics)。根目录 README 用来介绍项目价值、用法与贡献方式。
- 外链边界依据 [Google 链接最佳实践](https://developers.google.com/search/docs/crawling-indexing/links-crawlable)和 [Google 垃圾内容政策](https://developers.google.com/search/docs/essentials/spam-policies)。Google 将主要为操纵排名而创建链接的做法列为链接垃圾；本方案不采用批量建仓、批量评论、购买链接或强制互链。

## 发布前检查

- 已通过 GitHub 仓库接口确认：`yjkhxy/birthdayfreebieslist.com` 为公开仓库，默认分支为 `main`，Issues 已开启。当前 Website 为空、Topics 为空，Description 仍为初始简介；这些设置尚未修改。
- 核对待提交范围：`README.md`、`CONTRIBUTING.md`、纠错 issue 表单及本指引。不要把网站私有源码、环境文件或知识库原文搬进文档仓库。
- 按项目约定，改动经用户确认后再提交并推送。本文交付时尚未完成提交、推送或远端仓库设置。
- 推送后打开仓库首页，检查 README 表格、链接、贡献指南和 issue 表单；表单只有到达 GitHub 默认分支后才能使用。

## 仓库 About 建议

发布 README 后配置以下字段；这些是待执行建议，不代表远端设置已经修改。

| 字段 | 建议值 |
| --- | --- |
| Description | Practical guide to US birthday freebies and rewards: signup deadlines, purchase conditions, brand guides, and redemption checklists. |
| Website | `https://birthdayfreebieslist.com/` |
| Topics | `birthday-freebies`, `birthday-rewards`, `freebies`, `rewards-programs`, `shopping`, `consumer-guide` |

Topics 选与内容真正相关的词，不堆叠不相关热门技术标签。不把仓库标成 awesome 精选集、开源应用或免费 API，除非日后内容确实满足相应定位。

## 外链与分享方式

- README 主入口使用品牌名和清晰动作；分类链接回答不同需求，品牌示例解释条件差异，避免重复堆积相同关键词。
- 保持正文链接为不带追踪参数的 HTTPS 正式地址。网站 canonical 应指向对应正式页面；GitHub 自身页面的 canonical 和链接属性由平台控制，不能通过 README 修改。
- 网站上线、规则变化或发现错误时更新文档；不要靠无意义提交制造活跃度。品牌条目是否存在，不等于当前有福利，更不等于已核验免费。
- 如需推广，可在个人 GitHub 主页或确实相关的资源清单中介绍本指南；先读对方收录规则，只在它能补充实用信息时提交。是否收录由维护者决定，本次没有向任何其他仓库或社区发送内容。
- 可用的英文简介：`A practical birthday rewards guide with signup checks, purchase-condition explanations, and links to category and brand pages. Useful when planning which offers to verify before your birthday month.`
- 第三方平台可能为外链添加 `nofollow` 或 `ugc` 等属性；即使存在可点击链接，也不能据此断言会传递排名信号。不要承诺收录时间、权重分值或关键词名次。

## 复检与衡量

- 本次线上基线：2026-11-10 检查首页、无需消费页、5 个分类页、delivery 页、6 个品牌页及 about/contact/disclosure 共 17 个 HTML 页面，均 HTTP 200，canonical 与对应正式地址一致。
- `robots.txt` 返回 200，允许抓取并声明正式 sitemap；`sitemap.xml` 返回 200，含 173 个 URL，未发现 state/city 路径。发布文档不需要为网站 sitemap 添加 GitHub URL。
- 发布后再检一次 README 的实际落地链接、canonical、robots 和 sitemap。HTTP 200 或进入 sitemap 都不代表已被 Google 收录。
- 首次发布记录提交日期及网站现有访问基线；第 7、28 天检查来自 `github.com` 的推荐访问、落地页和用户行为。若现有分析工具提供这些数据再使用；先确认是否保留 referrer，不虚构访问统计。
- 在 GSC 对比品牌词和相关落地页的展示、点击及收录变化，同时记录其他网站改动。GSC 不提供“某条 GitHub 链接贡献了多少权重”的指标，也不能仅凭同期增长判断因果。
- 维护节奏：有官方规则变化立即修正；每月检查链接与示例，每年复核带年份的站内入口。把读者报错及有价值的补充整理为后续维护任务。
