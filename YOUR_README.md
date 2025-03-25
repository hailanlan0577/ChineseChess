# 中国象棋 - 个人部署说明

这是一个基于Qt开发的跨平台中国象棋游戏。本仓库是从[XMuli/ChineseChess](https://github.com/XMuli/ChineseChess)项目fork而来，用于个人学习和使用。

## 功能特点

- 玩家与自己对战
- 玩家与电脑AI对战
- 多人网络对战(可跨不同系统)
- 对战计时
- 悔棋（可多步）
- 下棋轨迹显示
- 支持Windows/Linux/MacOS等多个平台

## 如何构建和运行

### 依赖项
- Qt 5.12.11 或更高版本
- cmake 或 qmake 构建工具

### 在Ubuntu/Debian系统上构建
```bash
# 安装依赖
sudo apt install cmake qtbase5-dev qt5-default libqt5svg5-dev qtmultimedia5-dev qttools5-dev libqt5x11extras5-dev

# 克隆仓库
git clone https://github.com/hailanlan0577/ChineseChess.git

# 构建
cd ChineseChess
mkdir build && cd build
cmake ..  # 或者使用 qmake ..
make
```

### 在Windows上构建
1. 安装Qt和Qt Creator
2. 使用Qt Creator打开`ChineseChess.pro`文件
3. 点击构建和运行

### 在MacOS上构建
1. 安装Qt和Qt Creator
2. 使用Qt Creator打开`ChineseChess.pro`文件或使用命令行构建
3. 点击构建和运行

## 目录结构说明
- `ChessBoard.*` - 棋盘相关类
- `ChessPieces.*` - 棋子相关类
- `MachineGame.*` - AI对战相关类
- `NetworkGame.*` - 网络对战相关类
- `ChooseMainWindow.*` - 主界面选择窗口
- `resources/` - 资源文件夹，包含图片、音效等

## 注意事项
- 对于网络对战功能，需要确保网络连接正常
- 在某些系统上可能需要单独安装音频库以支持音效功能

## 联系方式
如有任何问题，请在GitHub上提交issue或联系原作者。

## 致谢
感谢原作者[XMuli](https://github.com/XMuli)及所有贡献者的工作。
