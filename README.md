# 🎨 AI提示词拼接工具（模块化多选版）

一个通过模块化组合的方式快速拼接生成AI提示词的轻量级Web工具。
<img width="1496" height="1223" alt="image" src="https://github.com/user-attachments/assets/41fd247b-72d6-4f6e-9a94-a6422bfd01fb" />
<img width="1494" height="1151" alt="image" src="https://github.com/user-attachments/assets/5e3556e8-35cd-49c2-8a8b-9ab1218fcb90" />

## ✨ 功能特点

- 📁 **JSON文件驱动**：通过上传JSON文件自定义提示词模块
- 🏷️ **模块化选择**：按主题分类的标签式选择界面
- ✅ **多选支持**：每个模块支持选择多个标签
- 📋 **一键复制**：生成的提示词可一键复制到剪贴板
- 📱 **响应式设计**：适配桌面和移动设备
- 🎯 **实时预览**：即时查看拼接结果

## [🚀 快速开始](https://starttown.github.io/AI_prompt-generator/)

1. **下载项目**

'''bash

git clone https://github.com/starttown/AI_prompt-generator.git

cd AI_prompt-generator

'''

2. **准备JSON文件**
   创建符合格式的JSON文件（参考 [test.json](test.json)）

3. **使用步骤**
   
   - 点击"选择JSON文件"上传配置文件
   - 在各模块中选择需要的标签（可多选）
   - 点击"拼接提示词"生成结果
   - 点击"复制到剪贴板"复制结果

## 📄 JSON文件格式


`[
{
“module”: “模块名称”,
“description”: “模块描述（可选）”,
“options”: [
“选项1”,
“选项2”,
“选项3”
]
},
{
“module”: “另一个模块”,
“options”: [
“选项A”,
“选项B”
]
}
]`

### 格式要求：

- 必须是有效的JSON数组
- 每个模块必须包含：
  - `module`：字符串（模块名称）
  - `options`：字符串数组（选项列表）
- 可选字段：
  - `description`：模块描述文本

## 📁 项目结构

AI_prompt-generator/
├── index.html # 主程序文件
├── test.json # 示例JSON文件
└── README.md # 项目说明

## 🛠️ 技术栈

- HTML5
- CSS3（原生变量）
- Vanilla JavaScript
- File API
- Clipboard API

## 🤝 贡献指南

欢迎提交Issue和Pull Request！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

## 📝 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 🌟 致谢

感谢所有为这个项目做出贡献的开发者！



项目使用说明

文件上传：

点击"选择JSON文件"按钮
选择符合格式的JSON文件（如提供的test.json）

标签选择：

每个模块显示为独立的卡片
点击标签进行多选/取消选择
选中的标签会高亮显示

生成提示词：

选择完所需标签后点击"拼接提示词"
生成的提示词格式：[模块名]: 选项1, 选项2; [模块名]: 选项3

复制结果：

点击"复制到剪贴板"按钮
成功复制后按钮会显示"✅ 已复制!"状态
