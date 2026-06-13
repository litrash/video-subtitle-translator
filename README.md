# 🎬 实时视频翻译字幕

一个实时识别视频语音并翻译成中文字幕的工具，支持Chrome浏览器插件和iOS Safari网页版。

## 🌟 在线体验

**iOS/手机用户**：直接访问 [https://你的用户名.github.io/video-subtitle-translator/](https://你的用户名.github.io/video-subtitle-translator/)

**电脑用户**：下载Chrome插件或使用网页版

## ✨ 功能特点

- ✅ 实时语音识别（使用浏览器内置Web Speech API）
- ✅ 自动翻译成中文
- ✅ 支持多种语言识别（英语、日语、韩语等）
- ✅ 两种使用方式：Chrome插件 / iOS网页版
- ✅ 完全免费，无需API密钥

## 📱 使用方式

### 方式一：iOS Safari 网页版（推荐手机用户）

1. 用 iPhone Safari 浏览器访问：[在线地址](https://你的用户名.github.io/video-subtitle-translator/)
2. 点击"启动语音识别"
3. 允许麦克风权限
4. 播放视频，字幕实时显示

**提示**：可以添加到主屏幕，像App一样使用

### 方式二：Chrome浏览器插件

1. 下载项目文件
2. 打开 `chrome://extensions/`
3. 开启"开发者模式"
4. 加载 `video-subtitle-translator` 文件夹
5. 在视频网站使用

详细说明请查看 [快速测试指南.md](快速测试指南.md)

## 🎯 支持的网站

- ✅ YouTube
- ✅ 哔哩哔哩
- ✅ 腾讯视频
- ✅ 所有HTML5视频网站

## 🛠️ 技术栈

- **语音识别**：Web Speech API
- **翻译**：有道翻译API
- **前端**：原生JavaScript + HTML5 + CSS3
- **浏览器**：Chrome/Safari

## ⚠️ 注意事项

- 需要允许麦克风权限
- 当前版本使用麦克风识别环境声音（不是直接捕获视频音频）
- 建议在安静环境中使用
- 需要网络连接（翻译功能）

## 📂 项目结构

```
video-subtitle-translator/
├── ios-webapp.html           # iOS网页版（主要文件）
├── index.html               # 首页重定向
├── manifest.json            # Chrome插件配置
├── content.js              # 插件内容脚本
├── background.js           # 插件后台脚本
├── popup.html              # 插件弹窗
├── README.md               # 项目说明
└── iOS使用指南.md          # 详细使用说明
```

## 🚀 本地部署

### 快速启动

1. 克隆项目：
```bash
git clone https://github.com/你的用户名/video-subtitle-translator.git
cd video-subtitle-translator
```

2. 启动本地服务器：
- Windows：双击 `start-server.bat`
- Mac/Linux：运行 `./start-server.sh`

3. 访问 `http://localhost:8000/ios-webapp.html`

### 部署到GitHub Pages

1. Fork本项目
2. 在仓库设置中启用 GitHub Pages
3. 选择 `main` 分支作为源
4. 访问 `https://你的用户名.github.io/video-subtitle-translator/`

## 🔮 未来计划

- [ ] 直接捕获视频音频（不依赖麦克风）
- [ ] 本地语音识别模型（Whisper.cpp）
- [ ] 更多翻译API选项
- [ ] 字幕样式自定义
- [ ] 字幕导出为SRT文件
- [ ] Firefox浏览器支持

## 📄 许可证

MIT License

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📮 联系方式

如有问题或建议，请提交 Issue。

---

**开发日期**: 2026年6月  
**版本**: 1.0.0  
**作者**: Claude Code
