# 上线指南：vape-hw-consult 落地页

## 1. 免费发布到 GitHub Pages
1. 注册/登录 GitHub，新建公开仓库，例如 `vape-hw-consult`。
2. 上传 `index.html`（放在仓库根目录）。命令行方式：
   ```bash
   cd /workspace/landing/vape-hw-consult
   git init && git add index.html && git commit -m "landing page"
   git branch -M main
   git remote add origin https://github.com/<你的用户名>/vape-hw-consult.git
   git push -u origin main
   ```
3. 仓库 Settings → Pages → Source 选 “Deploy from a branch”，分支 `main`，目录 `/ (root)`，保存。
4. 1–3 分钟后访问 `https://<你的用户名>.github.io/vape-hw-consult/`。
5. **上线前必须**：把 `index.html` 里表单的 `action="https://formsubmit.co/YOUR_EMAIL_HERE"`（已标注 TODO）换成你的邮箱或 Formspree 地址；FormSubmit 首次提交会发确认邮件，点确认后才生效。自己先测试提交一次。

## 2. 可选：自定义域名（约 $10/年）
- 在 Cloudflare Registrar / Namecheap / Porkbun 购买 `.com`（约 $10/年），如 `szhardwareconsult.com`。
- DNS 添加：`CNAME  www → <用户名>.github.io`；根域名添加 4 条 A 记录：185.199.108.153 / 109.153 / 110.153 / 111.153。
- GitHub Pages 设置里填自定义域名，勾选 “Enforce HTTPS”。
- 好处：可信度更高，邮箱也可以用同域名（如 Zoho 免费版）。

## 3. $30–40 小额广告测试计划（2 周）
> 注意：Reddit、LinkedIn、Google、Meta 对电子烟/大麻相关广告有严格限制，甚至禁止。广告文案只强调“硬件供应链/制造咨询”，避免出现 vape、THC、cannabis 等字样的产品推广，提前阅读各平台政策；被拒就转为自然发帖。

| 渠道 | 预算 | 定向 | 文案方向 |
|---|---|---|---|
| LinkedIn | ~$20（约 7–10 天，单价高，点击可能只有 5–10 个） | 职位：Founder / Product / Sourcing / Operations；行业：Consumer Goods、Tobacco、Cannabis（如可选）；地区：美国、加拿大、英国、欧盟 | “在深圳采购消费电子硬件？下单 MOQ 前先拿到成本模型和合规清单。” |
| Reddit | ~$15–20 | 社区兴趣：entrepreneur、smallbusiness、manufacturing、ecommerce | “ODM 产品经理出身，帮海外品牌做深圳硬件采购与成本建模，招募首批客户。” |
| 免费补充 | $0 | LinkedIn 个人动态、r/cannabusiness 等允许的社区（遵守版规）、行业群 | 分享一篇“陶瓷一次性设备成本构成”科普，附落地页链接 |

- 每个链接加 UTM 参数，如 `?utm_source=reddit&utm_campaign=test1`，方便区分来源（可加免费的 GoatCounter / Cloudflare Web Analytics）。
- 第 1 周后看点击率，表现差的渠道停掉，预算集中到较好的渠道。

## 4. 成功指标
- **核心指标：2 周内收集 10 个有效邮箱**（真实公司邮箱优先）。
- 辅助：落地页转化率 ≥ 5%；至少 2 人同意 30 分钟介绍电话；至少 1 个付费 Sourcing Brief 意向。
- 判定：
  - ≥10 个邮箱 → 需求成立，开始一对一联系并试卖 $299 套餐；
  - 3–9 个 → 调整标题/价格/渠道再测 2 周；
  - <3 个 → 重新考虑定位（例如只做大麻硬件或只做电子烟）。

## 5. 合规提醒
- 只做硬件咨询，不涉及烟油、THC 油或任何受控物质；大麻相关客户需提供合法执照。
- 页面不写雇主名称、不编造客户、数据或评价。注意现雇主的劳动合同中是否有竞业/兼职条款。
