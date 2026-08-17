# dsh-diorama · DSH 角色舞台

<p align="center">
  <strong>雪乃·暖阳日常</strong> · <strong>隐秘年代志</strong><br>
  双角色立绘 + 表情贴纸 + 可编辑装饰看板 · DeepSeek Harness 皮肤插件
</p>

## ✨ 功能

- **两套角色皮肤**（右下角 dropdown 切换，含"官方默认"还原）
  - **雪乃 · 暖阳日常**：雪乃校服/杂志风双立绘 + 3 张表情贴纸
  - **隐秘年代志**：白毛/魔女双立绘 + 2 张表情贴纸
- **可编辑装饰看板**（点皮肤行右侧 ✎）：拖动移动、手柄缩放、旋转/不透明度滑块、坐标数值精调、底部/顶部 + 左/右锚定切换
- **自定义素材**：上传你自己的图片作为角色/贴纸
- **分享**：导出装饰包（素材 + 布局打包为 JSON），导入后自动切换到对应皮肤并打开看板，可直接继续调整
- **持久化**：皮肤选择与装饰配置存 localStorage，刷新不丢

## 安装

```sh
dsh plugin --profile web add -w dsh-diorama
```

然后重启：

```sh
dsh web
```

刷新浏览器，右下角出现皮肤切换按钮。

## 使用

1. 点右下角按钮 → 选择「雪乃 · 暖阳日常」或「隐秘年代志」
2. 再次打开菜单 → 点皮肤名右侧的 **✎** 进入装饰编辑器
3. 拖动/缩放/旋转角色与贴纸，或点「＋ 图片」上传自己的素材
4. 「导出包」下载分享文件，「导入包」加载别人分享的装饰

## 开发

插件为标准 DSH 双面结构（`dsh.bundle` + `dsh.client`），`lib/client.js` 为 `__ModuleLoader__` 格式，免构建。

```sh
# 本地安装调试
dsh plugin --profile web add link:$(pwd)
```

## 兼容性

- DeepSeek Harness `>= 0.1.0-rc.6`
- Node.js `>= 18`
- 现代 Chromium / WebKit

## License

MIT
