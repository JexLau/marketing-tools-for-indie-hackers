# LinkedIn智能DM系统

## 功能描述
智能化的LinkedIn私信发送系统，通过AI分析用户档案生成个性化消息，提高B2B销售和网络建设效率。

## 核心功能
- 👥 目标用户筛选
- 🎯 个性化消息生成
- 📈 发送进度跟踪
- 💬 回复率统计分析
- 🔄 自动跟进提醒

## 商业价值
- **B2B销售**: 精准触达决策者
- **人脉拓展**: 建立专业网络
- **招聘获客**: 寻找优质人才
- **合作机会**: 发现潜在合作伙伴

## 技术栈
- Python 3.8+
- Selenium WebDriver
- OpenAI GPT API
- BeautifulSoup4
- Pandas

## 安装指南
```bash
cd tools/02-linkedin-dm
pip install -r requirements.txt

# 下载ChromeDriver
# 配置环境变量
cp .env.example .env
```

## 配置说明
```env
LINKEDIN_EMAIL=your_email@example.com
LINKEDIN_PASSWORD=your_password
OPENAI_API_KEY=your_openai_api_key
TARGET_KEYWORDS=CTO,技术总监,产品经理
MESSAGE_TEMPLATE=您好，我注意到您在{company}担任{position}...
```

## 使用方法
```python
from linkedin_dm import LinkedInDM

# 初始化DM系统
dm_system = LinkedInDM()

# 搜索目标用户
targets = dm_system.search_users(
    keywords=["CTO", "技术总监"],
    location="北京",
    industry="互联网"
)

# 发送个性化消息
dm_system.send_personalized_messages(targets)
```

## 安全注意事项
- 遵守LinkedIn使用条款
- 控制发送频率避免账号限制
- 使用代理IP分散请求
- 定期更新User-Agent

## 法律声明
本工具仅供学习和合法商业用途，使用者需自行承担法律责任。 