# README

## 关于

使用 sveltekit 的 wails 模板

默认使用 pnpm 作为包管理器

## 实时开发与构建

使用 `wails dev` 进行实时开发

使用 `wails build` 构建发布版本

## 架构

### 资源/静态文件

对于图像、字体等资源，请放在 `src/assets` 目录下，并使用如下命令引入

```javascript
import logo from "path/to/logo.png
```

对于如 `manifest.json`, `favicon.ico` 之类的无需进行预处理的资源，请放入 `static` 目录下（在桌面应用程序中应该不需要这类资源？）

### 路径别名

请在`svelte.config.js`中定义路径别名。里面已经有两个已经定义好的路径别名，分别为 `@assets` 和 `@wailsjsMain`
