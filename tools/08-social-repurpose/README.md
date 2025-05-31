# 跨平台内容转换工具

## 功能描述
智能将一种平台的内容转换为适合其他平台的格式，实现内容的跨平台最大化利用和传播。

## 核心功能
- 🔄 多平台内容适配
- 📏 格式自动调整
- 🎨 视觉元素优化
- 📱 移动端适配
- 📊 转换效果分析

## 商业价值
- **效率提升**: 一次创作多平台使用
- **覆盖面扩大**: 触达不同平台用户
- **成本降低**: 减少重复内容创作
- **品牌一致性**: 保持跨平台品牌形象

## 支持平台
- Twitter ↔ LinkedIn
- Instagram ↔ Facebook
- YouTube ↔ TikTok
- Blog ↔ Medium
- Podcast ↔ Newsletter

## 技术栈
- Python 3.8+
- OpenAI GPT API
- Pillow (图像处理)
- MoviePy (视频处理)
- Platform APIs

## 安装指南
```bash
cd tools/08-social-repurpose
pip install -r requirements.txt
cp .env.example .env
```

## 配置说明
```env
OPENAI_API_KEY=your_openai_api_key
TWITTER_API_KEY=your_twitter_key
LINKEDIN_ACCESS_TOKEN=your_linkedin_token
INSTAGRAM_ACCESS_TOKEN=your_instagram_token
```

## 使用方法
```python
from social_repurpose import ContentConverter

converter = ContentConverter()
linkedin_post = converter.convert(
    content="Twitter thread content",
    from_platform="twitter",
    to_platform="linkedin"
)
``` 