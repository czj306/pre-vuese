# vue组件文档自动生成
> 基于 vuese

## 安装
```
npm install vuese -D
```

## 使用
### 生成文档
```
vuese gen
```

或则写入package.json中
```
"scripts": {
  "docs": "vuese gen"
}
```

```
npm run docs
```

### 使用配置文件
根据目录创建.vueserc 或 vuese.config.js
```
{
  "include": "./src/components/*/*.vue", // 包含的文件
  "outDir": "docs", // 文档的输出目录
  "markdownDir": "components",
  "title": "Component UI Api", // 生成组件文档index的title
  "exclude": ["node_modules/**/*.vue"] // 排除的文件，node_modules已被默认排除
}
```

### 预览组件文档
```
vuese serve --open
```

### 相应式预览单个组件文档
```
vuese preview ./src/components/*/*.vue
```
