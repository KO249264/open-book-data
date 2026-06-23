# open-book-data

考试刷题小程序「open-book」的**题库数据仓库**(纯数据,不含程序代码)。

程序代码在 👉 https://github.com/KO249264/open-book

## 用途

本仓库通过 jsDelivr CDN 给小程序提供题库数据,改完题目 push 即可生效,小程序无需重新发版:

```
https://cdn.jsdelivr.net/gh/KO249264/open-book-data@main/data/manifest.json
```

## 目录结构

```
data/
├── manifest.json          题库索引(有哪些题库 / 章节 / 试卷 / 资料)
├── banks/                 各题库的题目 JSON
│   ├── exam-demo/
│   └── jianzao-demo/
└── materials/             配套资料(PDF / 图片,可选)
```

## 如何更新题库

1. 在主项目里编辑 `data/` 下的 JSON;
2. 把 `data/` 同步到本仓库并 push;
3. jsDelivr 会在数分钟内刷新(也可用带 commit hash 的链接立即生效)。

> 题目 JSON 的字段格式见主项目 README 与 `mock/index.js` 说明。
