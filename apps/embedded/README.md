# 循迹繁星嵌入版星图

UniApp WebView 加载的精简版 stellarium-web-engine。

## 功能

- 星图渲染（WebAssembly）
- 天体搜索
- 天体详情弹窗
- 「我的星星」查询面板
- JS Bridge API

## JS Bridge API

```js
// 设置观测位置
XingJi.setStellariumLocation(lat, lng)

// 天体选中回调
XingJi.onObjectSelected(callback)

// 设置 API 基地址
XingJi.setApiBaseUrl('https://api.xingji.com')

// 搜索天体
const results = await XingJi.searchStar('天狼星')

// 查询我的星星
const result = await XingJi.queryMyStar('13800138000')
```

## 部署

将 index.html + 编译后的 stellarium-web-engine.js + .wasm 放在同一目录。
