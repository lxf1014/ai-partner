# 🤖 AI 智能伴侣 (AI Partner)

基于 Streamlit 和 DeepSeek 大语言模型构建的可交互 AI 伴侣 Web 应用。项目实现了高度自定义的角色设定、流式对话输出以及多会话的持久化管理，为用户提供拟真、流畅的陪伴体验。

## 🔗 在线体验
👉 **[点击这里体验在线 Demo](<这里填你后续部署的 Streamlit 链接>)** 
*(注：如遇网络问题，可在本地运行)*

## ✨ 核心功能

- **角色定制 (Customizable Persona)**：支持在侧边栏自定义 AI 伴侣的“昵称”与“性格”，通过动态构建 System Prompt，实现不同性格的对话风格。
- **多会话管理 (Session Management)**：支持新建、切换和删除历史会话，会话记录自动以 JSON 格式持久化保存至本地，防止数据丢失。
- **流式响应 (Streaming Output)**：对接 DeepSeek API，实现打字机式的流式输出，大幅降低用户等待焦虑，提升交互体验。
- **状态管理 (State Management)**：深度利用 Streamlit 的 'session_state'，解决页面重绘导致的数据丢失问题，保证聊天记录的连贯性。

## 🛠️ 技术栈

- **前端框架**：Streamlit
- **核心语言**：Python 3
- **大模型接口**：OpenAI SDK (调用 DeepSeek API)
- **数据存储**：JSON (本地文件存储)

## 🚀 本地运行指南

如果你想在本地运行此项目，请按照以下步骤操作：

1. **克隆仓库**
   ```bash
   git clone <你的GitHub仓库链接>
   cd <你的仓库名称>

2.**安装依赖**
  本项目需要安装 streamlit 和 openai 库：
  ```bash
  pip install streamlit
  pip install openai
  ```

3.**配置 API Key**
  本项目使用 DeepSeek 的 API。请确保你的系统环境中设置了对应的环境变量：
  ```bash
  Windows (CMD): set DEEPSEEK_API_KEY=你的API_KEY
  Mac/Linux: export DEEPSEEK_API_KEY=你的API_KEY
  ```

4.**启动应用**
运行以下命令启动 Streamlit 应用：
```bash
streamlit run ai_partner.py
```

5.**📂 项目结构**
```text
├── ai_partner.py    # 核心应用代码
├── sessions/             # (自动生成) 用于存放聊天记录的 JSON 文件夹
└── README.md             # 项目说明文档
```

markdown
