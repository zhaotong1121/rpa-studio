# RPA Studio

可视化拖拽式 RPA（机器人流程自动化）桌面工具，体验类似影刀。

与基于 Playwright/Selenium 的方案不同，QCloud RPA Studio 通过 **Chrome/Edge 浏览器插件** 直接操控用户日常使用的真实浏览器，没有自动化指纹，能有效规避网站反爬检测。

## 核心特性

- **可视化流程设计**：基于 React Flow 的拖拽画布，节点式编排自动化流程
- **真实浏览器自动化**：通过插件桥接控制 Chrome/Edge，支持 Ctrl+点击拾取页面元素、滑块验证码处理
- **Windows 桌面自动化**：基于 UIA/MSAA 的桌面控件拾取与操作，支持鼠标、键盘、快捷键
- **丰富的数据节点**：Python 代码、HTTP 请求、MySQL、Redis、变量与日志
- **任务调度与监控**：定时任务、运行监控窗口、邮件通知
- **开箱即用**：安装包内置 Python 3.12 运行时，新电脑无需另装 Python
- **自动更新**：基于 electron-updater，启动时自动检查新版本

## 架构

RPA Studio (Electron + React)  ←→  Python 引擎 (FastAPI :8765)  ←WebSocket→  浏览器插件  →  Chrome/Edge 标签页

## 技术栈

Electron 34 · React 18 · React Flow · Vite 6 · CodeMirror · Python 3.12 · FastAPI · electron-builder
