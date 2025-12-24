# Mouse-Trail
# 鼠标轨迹效果

## English

### Mouse-Trail

**[Online Demonstration (Click to Access)](https://www.rockaz.top/GitHub-Project-Demo/Mouse-Trail/)**  
*Note: The website server is located in China.*

A lightweight JavaScript library to quickly add interactive mouse trail effects to web projects, enhancing visual feedback and user experience with customizable trail styles.

![GitHub license](https://img.shields.io/github/license/add-qwq/Mouse-Trail?style=flat-square)

This library creates smooth mouse trails using HTML5 Canvas, with support for customizing trail duration, line width, shadow effects, and rainbow color transitions. It's designed for easy integration and flexible control over the visual presentation.

### Key Features

- **Canvas-based Rendering**: Uses HTML5 Canvas for smooth, high-performance trail drawing
- **Customizable Parameters**: Adjust trail duration, line width, shadow blur, and color effects
- **Rainbow Effect**: Optional rainbow color transition for dynamic visual feedback
- **Responsive Design**: Automatically adapts to window resizing
- **Controllable States**: Supports pause, resume, and destruction of the trail effect
- **Lightweight**: No external dependencies, easy to integrate into any web project

### Quick Start

#### Installation

1. Download the `mouse-trail.js` file from the repository
2. Include it in your HTML file:
   ```html
   <script src="path/to/mouse-trail.js"></script>
   ```

#### Basic Usage

Initialize the mouse trail effect with default settings:
```javascript
// Initialize with default configuration
MouseTrail.init();
```

#### Custom Initialization

Initialize with custom configuration:
```javascript
// Initialize with custom settings
MouseTrail.init({
  trailDuration: 500,    // Trail lasts 500ms
  lineWidth: 5,          // Line width 5px
  shadowBlur: 12,        // Shadow blur 12px
  rainbowEffect: false   // Disable rainbow effect (use white)
});
```

### Configuration Options

| Parameter        | Type    | Default Value | Description                                  |
|------------------|---------|---------------|----------------------------------------------|
| `trailDuration`  | Number  | 300           | Trail persistence time in milliseconds       |
| `lineWidth`      | Number  | 3             | Width of the trail line in pixels            |
| `shadowBlur`     | Number  | 9             | Blur radius of the trail shadow              |
| `rainbowEffect`  | Boolean | true          | Enable/disable rainbow color transition      |

### API Reference

#### `init(customConfig)`
Initializes the mouse trail effect. Accepts an optional configuration object to override defaults.

```javascript
// Example
MouseTrail.init({ lineWidth: 4 });
```

#### `updateConfig(newConfig)`
Dynamically updates the trail configuration after initialization.

```javascript
// Example: Change to red trail with longer duration
MouseTrail.updateConfig({
  trailDuration: 600,
  rainbowEffect: false
});
```

#### `pause()`
Pauses the trail effect (stops updating and drawing).

```javascript
MouseTrail.pause();
```

#### `resume()`
Resumes the trail effect after pausing.

```javascript
MouseTrail.resume();
```

#### `destroy()`
Completely removes the trail effect, cleans up the canvas, and removes event listeners.

```javascript
MouseTrail.destroy();
```

### Compatibility

Compatible with all modern browsers that support HTML5 Canvas and ES6 features, including:
- Chrome 57+
- Firefox 52+
- Edge 15+
- Safari 10+
- Opera 44+

### License

This project is licensed under the [Apache-2.0 license](LICENSE).

---

## 中文

### 鼠标轨迹效果

**[在线演示（点击访问）](https://www.rockaz.top/GitHub-Project-Demo/Mouse-Trail/)**  
*注：网站服务器位于中国。

一个轻量级JavaScript库，用于为Web项目快速添加交互式鼠标轨迹效果，通过可自定义的轨迹样式增强视觉反馈和用户体验。

![GitHub license](https://img.shields.io/github/license/add-qwq/Mouse-Trail?style=flat-square)

该库使用HTML5 Canvas绘制流畅的鼠标轨迹，支持自定义轨迹持续时间、线宽、阴影效果和彩虹色过渡。设计初衷是便于集成并能灵活控制视觉呈现效果。

### 核心功能

- **基于Canvas渲染**：使用HTML5 Canvas实现流畅、高性能的轨迹绘制
- **可自定义参数**：调整轨迹持续时间、线宽、阴影模糊度和颜色效果
- **彩虹效果**：可选的彩虹色过渡，提供动态视觉反馈
- **响应式设计**：自动适应窗口大小变化
- **状态可控**：支持轨迹效果的暂停、恢复和销毁
- **轻量无依赖**：无外部依赖，易于集成到任何Web项目

### 快速开始

#### 安装

1. 从仓库下载`mouse-trail.js`文件
2. 在HTML文件中引入：
   ```html
   <script src="path/to/mouse-trail.js"></script>
   ```

#### 基本使用

使用默认设置初始化鼠标轨迹效果：
```javascript
// 使用默认配置初始化
MouseTrail.init();
```

#### 自定义初始化

使用自定义配置初始化：
```javascript
// 使用自定义设置初始化
MouseTrail.init({
  trailDuration: 500,    // 轨迹持续500毫秒
  lineWidth: 5,          // 线宽5像素
  shadowBlur: 12,        // 阴影模糊12像素
  rainbowEffect: false   // 禁用彩虹效果（使用白色）
});
```

### 配置选项

| 参数名称         | 类型    | 默认值  | 描述说明                          |
|------------------|---------|---------|-----------------------------------|
| `trailDuration`  | 数字    | 300     | 轨迹持续时间（毫秒）              |
| `lineWidth`      | 数字    | 3       | 轨迹线宽（像素）                  |
| `shadowBlur`     | 数字    | 9       | 轨迹阴影的模糊半径                |
| `rainbowEffect`  | 布尔值  | true    | 启用/禁用彩虹色过渡效果           |

### API参考

#### `init(customConfig)`
初始化鼠标轨迹效果。接受可选的配置对象以覆盖默认值。

```javascript
// 示例
MouseTrail.init({ lineWidth: 4 });
```

#### `updateConfig(newConfig)`
初始化后动态更新轨迹配置。

```javascript
// 示例：改为红色轨迹并延长持续时间
MouseTrail.updateConfig({
  trailDuration: 600,
  rainbowEffect: false
});
```

#### `pause()`
暂停轨迹效果（停止更新和绘制）。

```javascript
MouseTrail.pause();
```

#### `resume()`
暂停后恢复轨迹效果。

```javascript
MouseTrail.resume();
```

#### `destroy()`
完全移除轨迹效果，清理画布并移除事件监听器。

```javascript
MouseTrail.destroy();
```

### 兼容性

兼容所有支持HTML5 Canvas和ES6特性的现代浏览器，包括：
- Chrome 57+
- Firefox 52+
- Edge 15+
- Safari 10+
- Opera 44+

### 许可证

本项目采用[Apache-2.0 许可证](LICENSE)授权。
