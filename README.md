# 饥荒 mods 文档中文模板

## 文件系统

- `docs/`
- `code/`
- `assets/`
  - `cache/`

## 配置

可以使用`window.gPageLink`和`window.gBlobLink`作为本地引用

```js
{
  docs: "docs/refDocs/",
  code: "code/refDocs/",
  cache: "assets/cache/refDocs/",
  exclude: ["README", "SUMMARY"],
  global: ["GLOBAL"],
  ext: ".lua",
  remoteRepos: [
    {
      docs: `${window.gPageLink}#/docs/DST/`,
      code: `${window.gBlobLink}code/DST/`,
      cache: `${window.gPageLink}assets/cache/DST/`,
      ext: ".lua",
    },
  ],
}
```
