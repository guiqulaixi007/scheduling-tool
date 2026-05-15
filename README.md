# 需求排期工具

一个轻量级的需求排期甘特图工具，支持多角色协作排期、依赖关系管理、实时协作，纯前端实现，单 HTML 文件零部署。

## 功能特性

- **多角色排期**：支持后端、前端、iOS、Android、测试工程师，以及自定义角色
- **甘特图可视化**：自动生成排期甘特图，开发/联调/测试进度一目了然
- **依赖关系管理**：角色间依赖勾选，自动顺延开始日期，环状依赖检测
- **测试角色锁底**：测试角色在甘特图中始终排在最下方，卡片列表支持拖拽排序
- **日期合法性校验**：完成日期不能早于开始日期，实时提醒
- **实时协作**：基于 Firebase Realtime Database，多人实时同步排期数据
- **数据导入导出**：JSON 格式导入导出，支持离线使用
- **节假日识别**：内置 2025-2026 中国法定节假日和调休数据，工作日计算准确
- **GitHub Pages 部署**：无需服务器，直接通过浏览器访问

## 在线访问

👉 [https://guiqulaixi007.github.io/scheduling-tool/scheduling-tool.html](https://guiqulaixi007.github.io/scheduling-tool/scheduling-tool.html)

## 使用方法

1. 打开工具页面，填写需求名称和评审日期
2. 点击"下一步"，添加参与角色（后端、前端、测试等）
3. 为每个角色填写开发/测试起止日期、SP 数、联调天数
4. 勾选依赖关系（如前端依赖后端完成后才能开始）
5. 点击"生成排期甘特图"，查看可视化排期结果
6. 可通过"开启协作"创建房间，分享链接给队友实时协作

## 技术栈

- 纯 HTML + CSS + JavaScript（单文件，无构建依赖）
- Firebase Realtime Database（实时协作，可选）
- HTML5 Drag & Drop API（卡片排序）
- GitHub Pages（静态部署）

## 项目结构

```
scheduling-tool/
├── scheduling-tool.html   # 主文件（包含全部 HTML/CSS/JS）
├── README.md              # 项目说明
└── .git/                  # Git 仓库
```

## 许可

MIT License