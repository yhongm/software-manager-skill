# Software Manager Skill

> 软件产品经理/软件开发经理知识技能 - 主动式产品咨询 + PRD生成 + Mermaid图表 + **一键生成可交互H5原型图**

## 概述

Software Manager Skill 是一款面向 Claude Code 的软件产品经理助手。它遵循**主动式产品咨询流程**，帮助用户完成从需求分析到PRD文档输出、再到**可交互H5原型图**的完整产品工作流。

### 核心能力

- **需求分析**: 通过三问确认法明确产品方向、平台形态和成熟度
- **多源搜索**: 同时调用网络搜索 + RAG本地知识库，确保信息全面
- **PRD生成**: 输出符合行业标准的完整产品需求文档
- **Mermaid图表**: 自动生成产品架构图、甘特图等
- **H5原型图**: 一键生成纯H5+CSS+JS可交互原型（无需Vue/React，直接浏览器打开）

### 适用场景

- 从0到1设计新产品
- 撰写产品需求文档（PRD）
- 产品路线图规划
- 竞品分析
- 敏捷开发流程咨询
- **生成可交互H5原型图（纯H5+CSS+JS，无需Vue/React）**

## 工作流程

```
确认需求 → 提问澄清 → 网络搜索 + RAG搜索 → 产品规划 → PRD文档保存本地 + Mermaid图表 + H5原型图
```

### 阶段一：确认需求

收到产品需求后，通过三个核心问题确认：
1. 产品方向（做什么、面向谁、解决什么问题）
2. 平台形态（APP/小程序/Web、C端/B端）
3. 成熟度（从0到1新产品的迭代）

### 阶段二：多源资料搜索

**网络搜索** - 使用 `WebSearch` 工具获取：
- 行业趋势和最新动态
- 竞品功能和用户评价
- 设计方法和案例研究

**RAG本地搜索** - 读取本地参考文档：
- `pm-responsibilities.md` - PM职责与职业素养
- `prd-template.md` - PRD文档模板
- `pm-framework.md` - 分析框架（AARRR/SWOT/Kano等）
- `mermaid-guide.md` - Mermaid图表规范

### 阶段三：产品规划

输出：
- 一句话产品定位
- MoSCoW优先级分类
- MVP范围定义

### 阶段四：PRD文档输出

输出完整PRD文档，包含：
- 概述（背景、定位、目标用户、成功标准）
- 用户与场景（用户画像、核心用例）
- 功能需求（功能列表、详细说明、验收标准）
- 非功能需求（性能、安全、兼容性）
- 数据埋点
- 风险与依赖
- 附录

**按需保存**: 用户明确要求时，才使用 Write 工具保存到 `~/projects/{产品名称}/PRD/`

### 阶段五：Mermaid图表

根据产品类型自动生成对应图表：
- 从0到1产品 → 架构图  + MVP甘特图
- 迭代类产品 → 状态流转图 + 迭代计划甘特图 + 时序图
- 竞品分析 → 功能对比矩阵 + 架构对比图
- 数据分析 → AARRR漏斗图 + 留存曲线

## 使用示例

### 示例1：设计一款运动APP

**用户输入**：
> 帮我设计一个运动类的软件

**Skill响应**：
> 好的，我理解你想设计一款运动类软件...
> 产品方向/平台形态/成熟度 - 三问
> ...
> PRD文档 + Mermaid图表
> PRD已保存到: `~/projects/running-app/PRD/running-app_PRD_v0.1.md`

### 示例2：产品经理知识咨询

**用户输入**：
> 什么是Kano模型？

**Skill响应**：
> Kano模型是需求优先级划分的经典方法...

## 触发关键词

```
产品经理|PRD|产品需求文档|需求分析|产品设计|产品路线图|竞品分析|
用户故事|敏捷开发|Scrum|产品从0到1|功能需求|非功能需求|
Kano模型|RICE评分|MoSCoW|产品架构|Mermaid|...
```

## 目录结构

```
software-manager-skill/
├── SKILL.md                      # 核心技能定义
├── README.md                     # 本文件
├── LICENSE                       # MIT License
└── references/                   # 本地知识库
    ├── pm-responsibilities.md    # PM职责与职业素养
    ├── prd-template.md          # PRD模板
    ├── sdlc-product-process.md   # 软件开发生命周期
    ├── mermaid-guide.md         # Mermaid图表规范
    ├── pm-framework.md          # PM分析框架
    ├── pm-skills.md             # PM技能体系
    ├── pm-career-path.md         # PM职业路径
    ├── agile-dev.md             # 敏捷开发实践
    ├── tailwind-core/           # Tailwind CSS核心文档
    ├── icon-libraries/          # 图标库资源（Heroicons/Lucide/Iconify）
    └── h5-prototype/            # H5移动端最佳实践
```

## 技术栈

- **框架**: Claude Code Skill System
- **搜索**: WebSearch + WebFetch + Grep/Read
- **文档**: Markdown + Mermaid
- **输出**: 本地文件保存

## 参考资源

### 官方文档
- [Atlassian Agile](https://www.atlassian.com/software-development-lifecycle)
- [Scrum Guide](https://www.scrumguides.org/)
- [Mermaid Documentation](https://mermaid.js.org/)
- [Tailwind CSS 中文文档](https://www.tailwindcss.cn/)

### 图标库
- [Heroicons](https://heroicons.com/) — MIT, 316图标
- [Lucide](https://lucide.dev/) — MIT, 1000+图标
- [Iconify](https://iconify.design/) — Apache 2.0, 200k+图标

### 产品经理社区
- [人人都是产品经理](https://www.woshipm.com/)
- [周菜花](https://www.zhouqicf.com/)
- [ProductBoard](https://www.productboard.com/)
- [Aha! Roadmap](https://www.aha.io/)

## 更新日志

### v2.2.0 (2026-04-24)
- 新增: 一键生成可交互H5原型图（纯H5+CSS+JS，无需Vue/React）
- 新增: Tailwind CSS核心文档爬取（utility-first/responsive-design/dark-mode/animation等9个文件）
- 新增: 图标库资源参考（Heroicons/Lucide/Iconify/SVGRepo）
- 新增: H5移动端最佳实践文档
- 评分: 99.0/100 A级

### v2.1.0 (2026-04-23)
- 重命名: skill名称从 product-manager 改为 software-manager-skill
- 同步更新文件夹名称

### v2.0.0 (2026-04-23)
- 修复: 阶段二增加网络搜索，不再只依赖RAG本地搜索
- 新增: 支持用户指定路径保存PRD文档
- 新增: README.md文档完善

### v1.0.0 (2026-04-23)
- 初始版本
- 支持主动式产品咨询流程
- PRD文档模板
- Mermaid图表生成

## 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 创建 Pull Request

## License

本项目采用 MIT License - 详见 [LICENSE](LICENSE) 文件

---

*Built with Claude Code*
