English version: see README_EN.md

[![English Version](https://img.shields.io/badge/English-README_EN.md-blue?logo=github)](README_EN.md)

# FinanceMCP - 专业金融数据MCP服务器 🚀

[![smithery badge](https://smithery.ai/badge/@guangxiangdebizi/FinanceMCP)](https://smithery.ai/server/@guangxiangdebizi/FinanceMCP)

**基于MCP协议的专业金融数据服务器，集成Tushare API，为Claude等AI助手提供实时金融数据和技术指标分析能力。**

## 📑 目录

- [🌟 公网免费服务](#-公网免费服务)
- [⚡ 核心特性](#-核心特性)
- [🛠️ 工具总览](#️-工具总览)
- [🎯 技术亮点](#-技术亮点)
- [🚀 快速开始](#-快速开始)
- [💡 示例问句](#-示例问句)
- [🔧 本地部署](#-本地部署)
- [📄 许可证](#-许可证)

## 🌟 公网免费服务

**🎉 无需部署，即开即用！**

<<<<<<< HEAD
我们提供多种公网免费服务方式：

### 🌐 Web在线体验版
**🚀 最简单的使用方式！**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3b6e2310-afb2-407d-805d-b1a6b9ff6ea6" />

访问我们的在线体验网站：**[http://106.14.205.176:3222/](http://106.14.205.176:3222/)**

- ✨ **零配置体验** - 无需任何配置，打开网页即用
- 🤖 **集成大模型** - 直接与AI助手对话，获取金融分析
- 💬 **智能交互** - 自然语言提问，实时获取金融数据
- 📱 **多端适配** - 支持电脑、手机、平板访问
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/40d435a5-741d-41f3-a471-56bd5386d132" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/188c7222-5d60-4076-9a65-664755fea6ee" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/73c6f17d-8133-458b-bb26-95422e33b4d7" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/64307568-70d5-425f-b3bc-2bf1d2e97ff2" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e3fbaa7f-25f0-4787-aab2-0d3caad1aeae" />

> ⚠️ **服务说明**：这是个人提供的小型服务器，请文明使用，切勿攻击或滥用。

### ⚙️ Claude桌面版配置
您也可以直接在Claude中配置使用，无需本地安装和API密钥：
=======
我们提供公网免费服务，您可以直接在Claude中配置使用，无需本地安装和API密钥：
>>>>>>> 

```json
{
  "mcpServers": {
    "finance-data-server": {
      "disabled": false,
      "timeout": 600,
      "type": "sse",
      "url": "http://106.14.205.176:3101/sse"
    }
  }
}
```

**服务优势：**
- ✅ **零配置** - 无需注册API密钥，直接使用
- ✅ **24/7稳定** - 服务器持续运行，随时可用
- ✅ **完整功能** - 支持所有12个工具和技术指标
- ✅ **实时数据** - 接入Tushare专业金融数据

> 📺 **使用教程**：[FinanceMCP完整使用指南](https://www.bilibili.com/video/BV1qeNnzEEQi/)

## ⚡ 核心特性

### 🧠 智能技术指标系统
- **智能数据预取** - 自动计算指标所需历史数据，消除NaN值
- **强制参数化** - 要求明确指定参数（如`macd(12,26,9)`），确保计算精确
- **模块化架构** - 参数解析、数据计算、指标引擎完全解耦
- **5大核心指标** - MACD、RSI、KDJ、BOLL、MA

### 🌍 全市场覆盖
- **9大市场** - A股、美股、港股、外汇、期货、基金、债券、期权
- **实时新闻** - 智能搜索7+主流财经媒体
- **宏观数据** - 11种经济指标（GDP、CPI、PPI、PMI等）
- **企业分析** - 财务三表、管理层信息、股东结构

## 🛠️ 工具总览

| 工具名称 | 功能描述 | 核心特性 |
|---------|---------|---------|
| 🕐 **current_timestamp** | 当前时间戳 | UTC+8时区，多格式输出 |
| 📰 **finance_news** | 财经新闻搜索 | 智能关键词搜索，7+媒体源覆盖 |
| 📈 **stock_data** | 股票+技术指标 | 9大市场 + 5种技术指标，智能预取 |
| 📊 **index_data** | 指数数据 | 主要市场指数历史数据 |
| 📉 **macro_econ** | 宏观经济数据 | 11种指标：GDP/CPI/PPI/PMI/Shibor等 |
| 🏢 **company_performance** | 公司财务分析 | 财务三表+管理层+基本面，13种数据类型 |
| 💰 **fund_data** | 基金数据 | 净值/持仓/分红，85%性能优化 |
| 👨‍💼 **fund_manager_by_name** | 基金经理查询 | 个人履历、管理基金列表 |
| 🪙 **convertible_bond** | 可转债数据 | 基础信息+发行数据+转股条款 |
| �� **block_trade** | 大宗交易 | 交易详情+双方营业部信息 |
| 💹 **money_flow** | 资金流向 | 主力/超大单/大中小单资金流分析 |
| 💰 **margin_trade** | 融资融券 | 4个API：标的/汇总/明细/做市借券 |

## 🎯 技术亮点

### 智能技术指标引擎
```
用户请求 → 参数解析 → 数据需求计算 → 扩展历史数据获取 → 指标计算 → 结果返回
```

**支持指标：**
- **MACD** `macd(12,26,9)` - 趋势分析
- **RSI** `rsi(14)` - 超买超卖判断  
- **KDJ** `kdj(9,3,3)` - 随机指标
- **BOLL** `boll(20,2)` - 布林带
- **MA** `ma(5/10/20/60)` - 移动平均线

### 核心技术优势
1. **智能预取机制** - 自动计算并获取指标所需的额外历史数据
2. **参数强制化** - 避免默认参数导致的计算差异
3. **高性能优化** - 基金数据查询性能提升85%（5.2s→0.8s）
4. **数据源整合** - 40+ Tushare API接口无缝集成

## 🚀 快速开始

### 1. 使用公网服务（推荐）
复制上面的JSON配置到Claude Desktop的配置文件中，重启Claude即可使用。

### 2. 配置文件位置
- **Windows**: `%APPDATA%\Claude\claude_desktop_config.json`
- **macOS**: `~/Library/Application Support/Claude/claude_desktop_config.json`

### 3. 开始使用
配置完成后，直接在Claude中提问即可！

## 💡 示例问句

### 📈 股票技术分析
```
"分析茅台(600519.SH)的技术状态，计算MACD(12,26,9)、RSI(14)、KDJ(9,3,3)"
"查看宁德时代(300750.SZ)的布林带BOLL(20,2)和四条均线MA(5,10,20,60)"
"苹果公司(AAPL)最近一个月的股价走势和MACD指标分析"
```

### 📊 综合分析
```
"全面分析比亚迪：财务状况、技术指标、资金流向、最新新闻"
"比较A股、美股、港股三大市场的表现和技术指标"
"评估宁德时代的投资价值：基本面+技术面+资金面"
```

### 📰 新闻与宏观
```
"搜索新能源汽车板块的最新政策和市场动态"
"分析当前宏观经济形势：GDP、CPI、PPI、PMI数据"
"美联储加息对中国股市的影响，相关新闻和数据"
```

### 💰 基金与债券
```
"查询沪深300ETF的最新净值和持仓结构"
"分析张坤管理的基金业绩表现"
"可转债市场概况和投资机会分析"
```

## 🔧 本地部署

如需本地部署，请按以下步骤操作：

### 环境要求
- **Node.js >= 18** - 从 [nodejs.org](https://nodejs.org/) 下载安装
- **Tushare API Token** - 访问 [tushare.pro](https://tushare.pro) 获取

### 获取Tushare API Token

1. **注册账户** - 访问 [tushare.pro](https://tushare.pro/register) 注册
2. **获取Token** - 在个人中心获取API Token
3. **积分说明** - 部分高级数据需要积分权限

**学生用户福利** - 可申请2000免费积分：
- 关注Tushare官方小红书并互动
- 加入学生QQ群：**290541801**
- 完善个人信息（学校邮箱/学生证）
- 提交申请材料给管理员

### 安装步骤

#### 方式1：通过Smithery安装（推荐）
```bash
npx -y @smithery/cli install @guangxiangdebizi/finance-mcp --client claude
```

#### 方式2：手动安装
```bash
# 1. 克隆项目
git clone https://github.com/guangxiangdebizi/FinanceMCP.git
cd FinanceMCP

# 2. 安装依赖
npm install

# 3. 配置API密钥
echo "TUSHARE_TOKEN=your_token_here" > .env
# 或者直接编辑 src/config.ts 文件

# 4. 构建项目
npm run build
```

### 启动服务器

**方式1：直接运行（stdio模式）**
```bash
node build/index.js
```

**方式2：使用Supergateway（推荐用于开发）**
```bash
npx supergateway --stdio "node build/index.js" --port 3100
```

### Claude配置

配置文件位置：
- **Windows**: `%APPDATA%\Claude\claude_desktop_config.json`
- **macOS**: `~/Library/Application Support/Claude/claude_desktop_config.json`

#### 配置1：stdio模式
```json
{
  "mcpServers": {
    "finance-data-server": {
      "command": "node",
      "args": ["C:/path/to/FinanceMCP/build/index.js"],
      "disabled": false,
      "autoApprove": [
        "current_timestamp",
        "finance_news",
        "stock_data",
        "index_data",
        "macro_econ",
        "company_performance",
        "fund_data",
        "fund_manager_by_name",
        "convertible_bond",
        "block_trade",
        "money_flow",
        "margin_trade"
      ]
    }
  }
}
```

#### 配置2：Supergateway模式（如使用端口3100）
```json
{
  "mcpServers": {
    "finance-data-server": {
      "url": "http://localhost:3100/sse",
      "type": "sse",
      "disabled": false,
      "timeout": 600,
      "autoApprove": [
        "current_timestamp",
        "finance_news",
        "stock_data",
        "index_data",
        "macro_econ",
        "company_performance",
        "fund_data",
        "fund_manager_by_name",
        "convertible_bond",
        "block_trade",
        "money_flow",
        "margin_trade"
      ]
    }
  }
}
```

### 验证安装
配置完成后，重启Claude Desktop，然后询问："获取当前时间"，如果返回时间信息说明安装成功。

## 📄 许可证

本项目采用MIT许可证。详情请参见 [LICENSE](LICENSE) 文件。

---

**👨‍💻 作者**：陈星宇 (Xingyu Chen)  
**📧 邮箱**：guangxiangdebizi@gmail.com  
**🔗 GitHub**：[guangxiangdebizi](https://github.com/guangxiangdebizi)

⭐ 如果这个项目对您有帮助，请给我们一个Star！
