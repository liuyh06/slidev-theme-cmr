# CMR 中文技术演示主题

白底、深蓝、45° 半透明叠放方块，支持中英文章节页和 18 种可复用布局。英伟达介绍是示例内容，主题不绑定英伟达品牌。

[在线预览](https://liuyh06.github.io/slidev-theme-cmr/) · [18 页示例源稿](./example.md) · [英文与组件说明](./README.md)

## 使用

```bash
git clone https://github.com/liuyh06/slidev-theme-cmr.git
cd slidev-theme-cmr
npm install
npm run dev
```

需要 Node.js >=22.22。示例图片从英伟达官方站点加载，需要网络。其他项目可以先通过 `npm install -D github:liuyh06/slidev-theme-cmr` 安装，再设置 `theme: cmr`。npm 首次发布后可直接安装 `slidev-theme-cmr`，是否已发布请查看 npm。

`npm run starter` 打开通用 10 页写作起始稿；`example.md` 为扩展的 18 页完整布局示例。

## 布局和素材

18 种布局、组件参数和插槽见英文 README。原稿版式对应关系见 [覆盖清单](./docs/layout-coverage.md)。主题保留了方块的旋转角度、透明度和位置，不包含原答辩正文、校徽、专有字体及私有截图。

主题默认使用本地完整中文字体。建议安装 Noto Sans CJK SC；也可配置 `--cmr-font` 与 headmatter 中的 `fonts.sans`。示例样式限定在 `nvidia-demo` 类内，不影响普通演示。

## 发布与许可

GitHub 仓库、npm 包发布、Slidev 社区主题库收录是独立步骤。详见 [发布说明](./docs/publishing.md)。代码采用 MIT；第三方图片、名称和商标不包含在 MIT 授权中，见 [第三方说明](./THIRD_PARTY_NOTICES.md)。
