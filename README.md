# 学习通自动刷课脚本


专为超星学习通（Chaoxing MOOC）设计的智能刷课工具，支持自动播放、倍速播放、防暂停等多项功能。

使用deepseek进行优化，原脚本地址(https://greasyfork.org/zh-CN/users/1398926-hu89h-lee)

## 📌 功能特性

- 🚀 **自动连续播放**
  - 无缝衔接章节视频
  - 自动跳过章节测试
  - 智能重试机制（最大重试次数3次）

- ⚡ **2倍速播放**
  - 强制锁定播放速度
  - 防止平台重置速率
  - 支持自定义修改播放速度

- 🛡️ **防暂停机制**
  - 拦截暂停指令
  - 自动恢复播放
  - 无视答题弹窗干扰

- 🔄 **智能页面监控**
  - 实时检测DOM变化
  - 自动适应页面更新
  - 控制台日志追踪

- 🎮 **可视化控制面板**
  - 一键启用/关闭功能
  - 实时状态反馈
  - 浮动控制按钮

## 📥 安装指南&&使用教程

### 环境要求
- 浏览器：Chrome 85+ / Firefox 80+ / Edge 90+

### 使用教程
- 打开学习通你要刷的课时的视频界面
- 按下F12，转至console（控制台）
- 粘贴脚本代码按下回车

## 🎮 使用说明

### 控制面板
![界面预览](https://via.placeholder.com/400x200?text=脚本界面预览)

- **防暂停按钮**  
  点击切换防暂停功能，启用后按钮变为绿色

- **自动下一节**  
  启用后视频结束自动跳转下一章节

- 状态栏  
  实时显示脚本运行状态和错误信息

### 快捷键
| 功能               | 快捷键       |
|--------------------|-------------|
| 切换防暂停模式     | Alt+P       |
| 切换自动下一节     | Alt+N       |
| 手动跳转下一节     | Alt+→       |

## ⚙️ 配置参数

修改脚本代码中的`CONFIG`对象自定义设置：
```javascript
const CONFIG = {
    TARGET_PLAYBACK_RATE: 2.0,   // 播放速度（建议1.0-2.0）
    MAX_RETRY: 3,                // 初始化最大重试次数
    INIT_CHECK_INTERVAL: 2000,   // 初始化检测间隔(ms)
    OBSERVER_DELAY: 3000         // 页面监控延迟(ms)
};
```

## 注意

本README文档及脚本均由deepseek-r1生成或优化


