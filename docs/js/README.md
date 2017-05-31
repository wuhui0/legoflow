# JS

本章节主要介绍 JavaScript 模块 相关功能

# 注意

JavaScript 模块主要由 webpack 管理，开发 / 构建工作流会自动获取项目目录 `/src/js/` 路径下 第一层 JS 文件（ 但不包括子文件夹下 JS 文件 或 带下划线前缀的 JS 文件 ）作为依赖入口，进行依赖链的热刷新

* 项目目录 `/src/js/` 第一层（ 不包括子文件夹 ）路径下若新增 JS 文件，需要 **重启工作流**，使新增文件成为依赖入口，构建新的依赖链，JS 模块功能才生效

* 项目目录 `/src/js/*.js` 为入口文件 ( 带下划线前缀的 JS 文件除外 )，**不应相互依赖**