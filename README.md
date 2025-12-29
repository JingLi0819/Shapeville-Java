
# 🎮 Shapeville - 互动图形学习游戏

[![Java](https://img.shields.io/badge/Java-8+-orange.svg)](https://www.oracle.com/java/)
[![Swing](https://img.shields.io/badge/Swing-GUI-blue.svg)](https://docs.oracle.com/javase/tutorial/uiswing/)
[![Maven](https://img.shields.io/badge/Maven-Project-red.svg)](https://maven.apache.org/)

一个基于Java Swing开发的**教育图形识别游戏**，专为儿童和几何学习初学者设计。通过6个精心设计的互动任务，让学习几何图形变得生动有趣！

## ✨ 项目亮点

- 🎨 **精美UI设计** - 采用渐变色彩、现代化界面布局
- ♿ **无障碍支持** - 内置色盲模式，确保所有用户都能享受游戏
- 🎯 **6个互动任务** - 从2D图形到3D立体，循序渐进的学习体验
- 📊 **实时进度跟踪** - 进度条和得分系统，激励用户持续学习
- 🔀 **难度选择** - 基础/高级模式，适应不同学习需求

## 🖼️ 运行界面展示

### 🏠 主界面
清新简洁的主界面，提供直观的任务选择入口。

![主界面](bin/images/README/images/img.png)

### 📚 学习任务概览
6个精心设计的学习模块，涵盖几何图形的各个方面。

![任务概览](bin/images/README/images/img_1.png)

### 🔺 任务1：图形识别
学习识别各种2D和3D图形，支持基础和高级两种难度模式。

![图形识别](bin/images/README/images/img_2.png)

### 📐 任务2：角度计算
通过互动方式学习角度的概念和计算方法。

![角度计算](bin/images/README/images/img_3.png)

### 📏 任务3：面积计算
掌握各种图形的面积计算公式和应用。

![面积计算](bin/images/README/images/img_4.png)

### 🔄 任务4：图形变换
学习平移、旋转、对称等图形变换概念。

![图形变换](bin/images/README/images/img_5.png)

### 🧩 任务5：组合图形
理解复杂图形的构成和分解。

![组合图形](bin/images/README/images/img_6.png)

### 🎲 任务6：高级挑战
综合运用所学知识解决复杂几何问题。

![高级挑战](bin/images/README/images/img_7.png)

## 🚀 快速开始

### 环境要求
- **Java 8 或更高版本**
- **Maven 3.6+** (可选，用于依赖管理)

### 运行方式

#### 方式一：IDEA中运行
1. 克隆或下载项目到本地
2. 在IntelliJ IDEA中打开项目
3. 找到 `MainWindow.java` 文件
4. 右键点击 `main` 方法 → "Run 'MainWindow.main()'"

#### 方式二：命令行运行
```bash
# 进入项目根目录
cd Shapeville-Java-GUI

# 编译项目
mkdir -p bin
javac -d bin -sourcepath src/main/java src/main/java/com/Shapeville/MainWindow.java

# 复制资源文件
cp -r src/main/resources/images bin/

# 运行程序
java -cp bin com.Shapeville.MainWindow
```

#### 方式三：Maven构建运行
```bash
# 使用Maven编译
mvn clean compile

# 运行程序
mvn exec:java -Dexec.mainClass="com.Shapeville.MainWindow"
```

## 🏗️ 项目架构

```
Shapeville-Java-GUI/
├── src/main/java/com/Shapeville/
│   ├── ShapevilleGUI.java          # 主窗口框架
│   ├── ShapevilleMainContent.java  # 主界面内容
│   ├── Task1Screen.java           # 任务1：图形识别
│   ├── Task2Screen.java           # 任务2：角度计算
│   ├── Task3Screen.java           # 任务3：面积计算
│   ├── Task4Screen.java           # 任务4：图形变换
│   ├── Task5Screen.java           # 任务5：组合图形
│   ├── Task6Screen.java           # 任务6：高级挑战
│   ├── ColorManager.java          # 颜色管理器(支持色盲模式)
│   ├── TopNavBarPanel.java        # 顶部导航栏
│   ├── BottomBarPanel.java        # 底部控制栏
│   └── ...                        # 其他UI组件
├── src/main/resources/
│   └── images/                    # 图像资源文件
├── pom.xml                        # Maven配置文件
└── README.md                      # 项目说明文档
```

## 🎯 核心功能

### 🎨 界面设计
- **渐变背景** - 动态渐变色彩，提升视觉体验
- **响应式布局** - 适配不同屏幕尺寸
- **现代化UI组件** - 自定义按钮、进度条、文本框等

### ♿ 无障碍特性
- **色盲模式** - 一键切换色盲友好配色方案
- **高对比度** - 确保视觉障碍用户的可访问性
- **智能状态管理** - 任务进行中自动锁定模式切换

### 📊 任务系统
- **进度跟踪** - 实时显示学习进度
- **得分系统** - 激励用户完成更多挑战
- **难度分级** - 基础/高级模式自由切换

### 🔧 技术特性
- **模块化设计** - 每个任务独立封装
- **状态管理** - 统一的颜色和界面状态管理
- **事件驱动** - 响应式的用户交互处理

## 🛠️ 技术栈

| 技术 | 版本 | 用途 |
|------|------|------|
| **Java** | 8+ | 核心开发语言 |
| **Swing** | - | GUI框架 |
| **Maven** | 3.6+ | 项目构建管理 |
| **Git** | - | 版本控制 |

## 📖 项目说明

### 设计理念
Shapeville旨在通过游戏化的方式让几何学习变得更有趣。项目采用了**渐进式学习**的设计理念，从简单的图形识别开始，逐步引导用户掌握更复杂的几何概念。

### 技术亮点
1. **颜色管理系统** - `ColorManager`类实现全局颜色控制，支持色盲模式动态切换
2. **界面刷新机制** - `ColorRefreshable`接口确保所有窗口实时响应颜色变更
3. **状态同步** - 多窗口状态智能管理，避免模式冲突
4. **资源管理** - 图片资源统一管理，支持动态加载

### 代码质量
- 遵循Java命名规范
- 模块化设计，高内聚低耦合
- 详细的中文注释
- 异常处理和用户体验优化

## 🔮 未来规划

- [ ] 添加更多几何图形类型
- [ ] 实现用户数据持久化
- [ ] 增加音效和动画效果
- [ ] 支持多语言界面
- [ ] 开发Web版本

## 🤝 贡献指南

欢迎提交Issue和Pull Request来改进项目！

1. Fork 本仓库
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的修改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个 Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 🙏 致谢

感谢所有为Java Swing生态系统做出贡献的开发者们！

---

**⭐ 如果这个项目对你有帮助，请给它一个Star！**
