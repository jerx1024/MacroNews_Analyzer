# MacroInsight - 宏观新闻分析工具

## 项目概述

MacroInsight 是一款专业的宏观经济新闻分析工具，利用 DeepSeek AI 模型对金融和经济新闻进行深度分析，评估其对不同资产类别的潜在市场影响。该工具为投资者、分析师和金融专业人士提供了结构化的多维度分析，帮助做出更明智的投资决策。

## 核心功能

### 1. 多维度影响分析
- **影响时长评估**：区分长期(数月至数年)、中期(数周至数月)和短期(数小时至数天)影响，基于经济理论和历史先例提供支持
- **影响方向与范围**：评估对股票、债券、商品、外汇和加密货币市场的影响方向（利好/利空/中性）
- **影响力度分析**：预测市场波动幅度，与历史相似事件对比，识别敏感因素和超预期情景
- **影响消退指标**：提供关键监测指标、建议监测时间窗口和潜在二次效应分析

### 2. 资产类别细分分析
- **股票市场**：细分行业影响差异
- **债券市场**：收益率曲线变化评估
- **商品市场**：能源、贵金属、农产品等不同商品类别分析
- **外汇市场**：主要货币对影响评估
- **加密货币市场**：主要加密货币影响分析
- **跨市场传导效应**：评估市场间的相互影响

### 3. 专业可视化
- **影响力度雷达图**：直观展示不同资产类别的影响程度
- **结构化表格**：条件格式化的资产类别影响表格
- **详细分析报告**：可导出完整的 Markdown 格式分析报告



## 安装指南

### 前提条件
- Python 3.8+
- DeepSeek API 密钥 ([申请地址](https://www.deepseek.com))

### 安装步骤

1. 克隆仓库
```
git clone https://github.com/Theclues/MacroNews_Analyzer.git
cd MacroInsight
```

2. 创建虚拟环境（可选但推荐）
```
python -m venv venv
source venv/bin/activate  # Linux/Mac
# 或
venv\Scripts\activate  # Windows
```

3. 安装依赖
```
pip install -r requirements.txt
```

4. 运行应用
```
streamlit run macroinsight.py
```

## 使用指南

### 基本使用流程
1. 启动应用后，在侧边栏输入您的 DeepSeek API 密钥
2. 在主界面文本区域粘贴宏观经济/金融新闻内容
3. 点击"分析新闻"按钮
4. 查看生成的多维度分析结果
5. 可选择下载完整分析报告（Markdown 格式）

### 高级选项
- **详细分析**：启用/禁用更深入的分析内容
- **包含可视化图表**：启用/禁用影响力度雷达图等可视化内容

## 技术架构

MacroInsight 采用以下技术栈构建：

- **前端界面**：Streamlit
- **数据可视化**：Plotly、Pandas
- **AI 模型**：DeepSeek API
- **数据处理**：Python 标准库、JSON

### 系统流程
1. 用户输入宏观新闻内容
2. 应用构建优化的分析提示词
3. 调用 DeepSeek API 进行深度分析
4. 解析返回的 JSON 结构化数据
5. 生成可视化图表和表格
6. 提供可下载的完整分析报告

## 分析示例

### 央行政策分析
对于央行降准等货币政策新闻，系统能够分析：
- 对股票市场的行业差异化影响
- 债券收益率曲线可能的变化
- 对商品市场和外汇市场的传导效应
- 历史相似政策的市场反应对比

### 通胀数据分析
对于通胀数据超预期等经济数据新闻，系统能够评估：
- 对不同资产类别的短期和长期影响
- 市场定价机制的调整预期
- 央行政策转向的可能性及其影响
- 投资组合调整建议

## 依赖项

```
streamlit
requests
pandas
plotly
```

## 版权信息

© 2025 MacroInsight 宏观新闻分析工具 | 基于DeepSeek AI模型

