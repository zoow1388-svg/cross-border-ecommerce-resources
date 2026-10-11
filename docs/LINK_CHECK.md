# 链接核验记录

**检查日期：2026-10-10（America/Chicago）。**

本记录对应首版 30 项官方资源与 4 篇中文补充教程。资源编号与 [README](../README.md) 一致。

## 方法与范围

- 逐项用网页工具打开官方页面、阅读相关正文，核对用途、适用场景和能够确认的限制；对中文教程检查实际操作内容。
- 在本机对最终清单中的外部链接执行 HTTP GET，跟随正常重定向，检查响应状态与页面标题；每个地址只请求一次，不执行自动重试或登录。
- 首轮检查 44 个地址；随后为 n8n 许可核验两个不同的官方候选地址，共执行 46 次自动 HTTP 请求。旧地址与失败候选保留在修正记录中。
- 最终 README 包含 **44 个不同外部链接**：30 个主资源、4 篇中文教程、9 个官方补充来源和 1 个品牌主页。主资源和教程不重复计数。
- 最终链接的本机结果为 **41 个 HTTP 200、1 个 HTTP 403、2 个连接被重置**。三个本机访问异常的主资源均另由网页工具成功返回官方正文，保留原访问限制。
- HTTP 200 只表示本次 HTTP 请求成功；内容核验独立记录。网页工具返回正文不代表本机访问故障已解决。

## 30 项官方资源

| 编号 | 官方页面 | 本机 GET | 正文与限制核验 |
| ---: | --- | --- | --- |
| 01 | [Amazon Seller University](https://sell.amazon.com/learn/seller-university) | HTTP 200 | 官方说明其为免费教育资源，覆盖发布、定价、履约与广告。 |
| 02 | [eBay Seller Center](https://www.ebay.com/sellercenter) | HTTP 200 | 卖家中心列出刊登、国际销售、退货、保护和费用资料。 |
| 03 | [Alibaba.com Seller Central](https://seller.alibaba.com/) | HTTP 200 | 官方卖家入口及 B2B 销售说明与条目用途一致。 |
| 04 | [Walmart Marketplace Learn](https://marketplacelearn.walmart.com/) | HTTP 200 | 官方学习中心提供商品、订单、回款和履约指南；论坛需登录。 |
| 05 | [Etsy Seller Handbook](https://www.etsy.com/seller-handbook) | HTTP 403 | 网页工具返回 Seller Handbook 正文，含开店、经营、品牌与服务文章；本机 HTTP 为 403。 |
| 06 | [Shopify 帮助中心](https://help.shopify.com/en) | HTTP 200 | 官方帮助中心列出商店、产品、订单、支付和配送栏目。 |
| 07 | [WooCommerce 官方文档](https://woocommerce.com/documentation/woocommerce/) | HTTP 200 | 官方文档列出商品、结账、配送、迁移和扩展资料。 |
| 08 | [Learn WordPress](https://learn.wordpress.org/) | HTTP 200 | 官方说明提供免费教育资源，含初学、设计和开发课程。 |
| 09 | [Cloudflare 基础文档](https://developers.cloudflare.com/fundamentals/) | HTTP 200 | 官方基础文档提供账户、产品接入、配置与限制入口。 |
| 10 | [PageSpeed Insights](https://pagespeed.web.dev/) | HTTP 200 | 已读取检测入口；官方说明区分移动/桌面、实验室/真实用户数据。 |
| 11 | [n8n 官方文档](https://docs.n8n.io/) | HTTP 200 | 官方文档说明工作流与 AI 集成；费用和许可另读官方页面。 |
| 12 | [Make Academy](https://academy.make.com/) | 连接被重置（无 HTTP 响应） | 网页工具返回官方课程与 FAQ；课程免费、每次报名访问期 6 个月；本机连接被重置。 |
| 13 | [Zapier 官方指南](https://zapier.com/resources/guides) | 连接被重置（无 HTTP 响应） | 网页工具返回官方指南正文；服务价格页另行核验；本机指南请求连接被重置。 |
| 14 | [DeepL Translator](https://www.deepl.com/en/translator) | HTTP 200 | 官方翻译入口及套餐页已读取；地区价格与免费额度未作通用结论。 |
| 15 | [Dify 官方文档](https://docs.dify.ai/en/home) | HTTP 200 | 官方说明知识库、Agent、工作流、云端 Sandbox 与自托管。 |
| 16 | [DHL 商业发票指南](https://www.dhl.com/discover/en-us/global-logistics-advice/essential-guides/how-to-prepare-a-commercial-invoice) | HTTP 200 | 官方正文列出商业发票填写字段，标明美国地区来源。 |
| 17 | [UPS 国际运输单证指南](https://www.ups.com/us/en/support/international-tools-resources/international-forms-certificates) | HTTP 200 | 官方正文解释商业发票、原产地与出口信息文件，并说明电子发票账户要求。 |
| 18 | [FedEx 清关文件指南](https://www.fedex.com/en-us/shipping/international/create-documents.html) | HTTP 200 | 官方正文提供清关文件与相关生成工具入口。 |
| 19 | [欧盟 Access2Markets](https://trade.ec.europa.eu/access-to-markets/en/home) | HTTP 200 | 欧盟官方入口可访问，提供贸易路线、关税和要求查询；未作具体税率判断。 |
| 20 | [英国 EORI 官方指南](https://www.gov.uk/eori) | HTTP 200 | 英国政府正文说明 EORI 需求与地区范围。 |
| 21 | [Google SEO 入门指南](https://developers.google.com/search/docs/fundamentals/seo-starter-guide) | HTTP 200 | Google 官方入门正文涵盖内容、标题、链接与图片等基础。 |
| 22 | [Google Search Console](https://support.google.com/webmasters/answer/9128668) | HTTP 200 | 官方明确服务免费，用于监测与排查自己网站的搜索表现。 |
| 23 | [Google Merchant Center 入门](https://support.google.com/merchants/answer/12159157) | HTTP 200 | 官方明确 Merchant Center 为免费工具，并提供商品与网站设置说明。 |
| 24 | [Google Analytics 4 入门](https://support.google.com/analytics/answer/10089681) | HTTP 200 | 官方入门正文介绍事件数据、网站与应用、首次接入和课程。 |
| 25 | [Similarweb](https://www.similarweb.com/) | HTTP 200 | 官方产品正文包含竞品、流量、市场与渠道研究用途。 |
| 26 | [PayPal 商家服务](https://www.paypal.com/c2/business) | HTTP 200 | 官方中国相关商家页面说明跨境收付产品；适用费用另读官方费率页。 |
| 27 | [Stripe 支持地区](https://stripe.com/global) | HTTP 200 | 官方正文列出商家支持地区；未推导个别主体可开户或具体交易费率。 |
| 28 | [Wise Business](https://wise.com/business/) | HTTP 200 | 官方企业页面与企业适用性说明已读取；未确认个别中国企业资格。 |
| 29 | [欧盟 VAT One Stop Shop](https://vat-one-stop-shop.ec.europa.eu/index_en) | HTTP 200 | 欧盟委员会正文提供电商 VAT、OSS/IOSS 相关说明。 |
| 30 | [英国 VAT 注册指南](https://www.gov.uk/register-for-vat) | HTTP 200 | 英国政府正文区分注册条件，包括境外企业相关规则；未给个体税务结论。 |

## 4 篇中文补充教程

| 教程 | 本机 GET | 实际价值与采用边界 |
| --- | --- | --- |
| [Alibaba.com 中文运营教程](https://www.toolbbs.com/sites/1454.html) | HTTP 200 | 已读入驻、产品资料、RFQ、询盘与报价步骤；不采用文章中的历史费用作当前报价。 |
| [WooCommerce 中文建站教程](https://www.toolbbs.com/sites/3264.html) | HTTP 200 | 已读商品、支付、配送及上线前测试订单步骤；不把示例服务器配置作为所有网站的必需配置。 |
| [n8n 中文邮件分类教程](https://www.toolbbs.com/sites/2127.html) | HTTP 200 | 已读邮件触发、AI 分类、分支、通知、测试及许可提醒；费用与许可另以当前官方资料为准。 |
| [Similarweb 中文竞品分析教程](https://www.toolbbs.com/sites/2821.html) | HTTP 200 | 已读流量趋势、国家、渠道、多竞品对比和估算数据边界。 |

## 官方补充来源

| 页面 | 本机 GET | 核验内容 |
| --- | --- | --- |
| [n8n 收费](https://n8n.io/pricing/) | HTTP 200 | 云端与自托管方案、执行量、企业功能；未复制固定报价。 |
| [n8n 许可](https://docs.n8n.io/n8n-community-license/community-license) | HTTP 200 | 现行 Community license 页面返回 Sustainable Use License 与企业许可说明。 正常重定向到 `https://docs.n8n.io/n8n-community-license`。 |
| [Zapier 收费](https://zapier.com/pricing) | HTTP 200 | 存在免费和付费计划，任务量与功能受计划约束。 |
| [DeepL 收费](https://www.deepl.com/en/pro) | HTTP 200 | 产品、字符、文档与团队权益按套餐和地区区分。 |
| [Dify 收费](https://dify.ai/pricing) | HTTP 200 | 套餐及使用限制；不视为免费无限模型调用。 |
| [Cloudflare 收费](https://www.cloudflare.com/plans/) | HTTP 200 | 不同产品和套餐的收费方式；不将网站接入与全部产品等同。 |
| [PageSpeed 官方说明](https://developers.google.com/speed/docs/insights/v5/about) | HTTP 200 | 实验室和真实用户数据、移动与桌面分析、数据不足等边界。 |
| [PayPal 商家费率](https://www.paypal.com/c2/business/paypal-business-fees) | HTTP 200 | 开户协议、地区、商业收款和兑换等费用的适用范围。 |
| [Wise 企业适用性](https://wise.com/help/articles/2977974/can-my-business-use-wise) | HTTP 200 | 企业主体、国家与业务类型等适用条件。 |

## 品牌主页与修正记录

- 品牌主页本机返回 HTTP 200，标题与品牌网站一致；主页链接仅在 README 放置一次。
- Shopify 旧的 manual 入口被官方重定向至帮助中心，本清单直接使用已核验的帮助中心地址。
- Merchant Center 和 PayPal 的旧资料入口存在官方重定向，本清单采用已核验的现行目标页面。
- n8n 旧路径 `/sustainable-use-license` 在本机返回 HTTP 404，已从清单移除。
- n8n 官方 GitHub `LICENSE.md` 候选链接由网页工具返回许可正文，但本机返回 HTTP 503，未保留为 README 链接。
- 从 n8n 当前官方文档索引找到 Community license 地址，已核验 HTTP 200 和许可正文；自动重定向仍停留在 n8n 官方文档域名。
- 网页工具访问 Stripe 地区页面时显示地区重定向，本机 GET 返回原全球页面。服务商地区跳转可随访问环境变化，未据此推导商家开户资格。

## 未解决问题与检查限制

1. 本机访问 Etsy 返回 HTTP 403；Make Academy 与 Zapier 指南连接被重置。尚未证明本机普通浏览器在同一网络下可以正常打开它们，正文仅由本次网页工具交叉核验。
2. 未对所有服务的国家资格、账户审核、个人报价、当前套餐额度、合同权益或业务特定限制逐一确认；README 已明确标注未确认项目。
3. 未执行真实开店、订阅、工作流运行、发货、付款、清关或税务申报，也未测试所有账户内部与动态交互功能。
4. 外部网站、价格和政策会变；本记录只代表上述日期的资料检查，不能据此保证后续持续可用。

## 发布前内容检查范围

发布前检查资源编号与分类数量、用途/人群/费用字段、四篇教程的真实地址、品牌主页链接次数、站内文档与目录锚点、重复链接、敏感信息及 Git 提交差异。该项目只包含文档，不涉及应用构建、启动或生产服务部署。
