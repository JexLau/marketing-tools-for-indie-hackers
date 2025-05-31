# 贡献指南

感谢您对营销工具集项目的关注！我们欢迎所有形式的贡献。

## 如何贡献

### 1. 选择工具
从[工具清单](README.md#工具清单)中选择一个您感兴趣的工具进行开发。

### 2. 开发环境设置
```bash
# 克隆仓库
git clone https://github.com/jexlau/marketing-tools-for-indie-hackers.git
cd marketing-tools-for-indie-hackers

# 创建新分支
git checkout -b feature/tool-name
```

### 3. 工具开发规范

#### 目录结构
每个工具应包含以下文件：
```
tools/xx-tool-name/
├── README.md           # 工具说明文档
├── requirements.txt    # Python依赖（如适用）
├── package.json       # Node.js依赖（如适用）
├── src/               # 源代码
├── docs/              # 详细文档
├── examples/          # 使用示例
└── tests/             # 测试文件
```

#### 代码规范
- **Python**: 遵循PEP 8规范，使用black格式化
- **JavaScript**: 遵循ESLint规范，使用Prettier格式化
- **注释**: 关键功能必须有注释
- **错误处理**: 完善的异常处理机制

#### 文档要求
每个工具的README.md包含：
1. 功能描述
2. 安装指南
3. 使用方法
4. API文档
5. 配置说明
6. 常见问题

### 4. 提交规范

#### Commit消息格式
```
type(scope): description

feat(twitter-monitor): 添加关键词监听功能
fix(linkedin-dm): 修复消息发送失败问题
docs(readme): 更新安装指南
```

#### Pull Request
1. 确保代码通过所有测试
2. 更新相关文档
3. 在PR描述中说明：
   - 实现的功能
   - 技术选型理由
   - 使用方法
   - 商业价值

### 5. 代码审查
- 所有PR需要至少一个维护者审查
- 确保代码质量和安全性
- 验证功能完整性

## 开发指南

### 环境要求
- Python 3.8+
- Node.js 16+
- Git

### 推荐工具
- VS Code + Python/JavaScript扩展
- Postman (API测试)
- Docker (容器化部署)

### 测试
```bash
# Python测试
pytest tests/

# JavaScript测试
npm test
```

## 社区规范
- 尊重所有贡献者
- 建设性的反馈和讨论
- 遵循开源精神
- 商业友好的MIT许可证

## 获得帮助
- 提交Issue描述问题
- 加入讨论区交流
- 查看现有文档和示例

让我们一起打造独立开发者的第一桶金工具集！🚀 