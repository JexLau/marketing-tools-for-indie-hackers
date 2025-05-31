# Twitter关键词监听 + AI自动回复

## 功能描述
实时监听Twitter上的特定关键词，并使用AI自动生成相关回复，帮助品牌和个人快速响应潜在客户。

## 核心功能
- 🔍 实时关键词监听
- 🤖 AI智能回复生成
- 📊 互动数据统计
- ⚙️ 自定义回复模板
- 🎯 精准用户定位

## 商业价值
- **客户获取**: 主动发现潜在客户
- **品牌曝光**: 增加品牌在社交媒体的可见度
- **销售转化**: 及时响应购买意向
- **竞争分析**: 监控竞争对手动态

## 技术栈
- Python 3.8+
- Twitter API v2
- OpenAI GPT API
- FastAPI
- SQLite/PostgreSQL

## 安装指南
```bash
# 克隆项目
git clone <repo-url>
cd tools/01-twitter-monitor

# 安装依赖
pip install -r requirements.txt

# 配置环境变量
cp .env.example .env
# 编辑.env文件，添加API密钥
```

## 配置说明
```env
TWITTER_BEARER_TOKEN=your_twitter_bearer_token
OPENAI_API_KEY=your_openai_api_key
KEYWORDS=SaaS,独立开发,创业
REPLY_TEMPLATE=感谢分享！我们的产品可能对您有帮助...
```

## 使用方法
```python
from twitter_monitor import TwitterMonitor

# 初始化监听器
monitor = TwitterMonitor(
    keywords=["SaaS", "独立开发"],
    auto_reply=True
)

# 开始监听
monitor.start_monitoring()
```

## API文档
详见 [API文档](docs/api.md)

## 部署指南
详见 [部署指南](docs/deployment.md)

## 注意事项
- 遵守Twitter API使用条款
- 合理控制回复频率
- 确保回复内容的相关性和价值

## 贡献
欢迎提交Issue和Pull Request！ 