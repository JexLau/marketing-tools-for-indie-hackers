# YouTube转文章发布系统

## 功能描述
将YouTube视频内容自动转换为高质量文章，并发布到多个平台，实现内容的最大化利用和传播。

## 核心功能
- 🎥 视频内容提取
- 📝 AI文章生成
- 🖼️ 自动配图
- 📤 多平台发布
- 📊 发布效果跟踪

## 商业价值
- **内容复用**: 一份内容多平台分发
- **SEO优化**: 文章形式更利于搜索引擎收录
- **受众扩展**: 覆盖不同内容消费习惯的用户
- **时间节省**: 自动化内容创作流程

## 技术栈
- Python 3.8+
- YouTube Data API
- OpenAI GPT API
- Whisper (语音转文字)
- WordPress API

## 安装指南
```bash
cd tools/06-youtube-to-article
pip install -r requirements.txt
cp .env.example .env
```

## 配置说明
```env
YOUTUBE_API_KEY=your_youtube_api_key
OPENAI_API_KEY=your_openai_api_key
WORDPRESS_URL=your-blog.com
WORDPRESS_USERNAME=your_username
WORDPRESS_PASSWORD=your_password
```

## 使用方法
```python
from youtube_to_article import YouTubeConverter

converter = YouTubeConverter()
article = converter.convert_video_to_article("video_url")
converter.publish_to_platforms(article)
``` 