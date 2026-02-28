# 在线工具集

纯前端实现的常用小工具集合，无需后端，数据仅在本机处理。

## 技术栈

- 纯 HTML + CSS + JavaScript，无构建
- 部署到 [Vercel](https://vercel.com) 静态站点

## 本地预览

用任意静态服务器打开根目录即可，例如：

```bash
# Python 3
python3 -m http.server 8080

# Node (需安装 npx)
npx serve .
```

然后访问 http://localhost:8080

## 工具列表

### 图片工具

- **占位图生成** — 按宽高、颜色、文字生成占位图
- **图片压缩** — 压缩 JPEG/PNG，可调质量
- **尺寸调整** — 按宽高或比例缩放图片
- **格式转换** — 转为 PNG / WebP / JPEG
- **二维码生成** — 输入文本生成二维码图片

### 编解码与格式化

- **Base64 编解码** — 支持中文与 Emoji
- **URL 编解码** — encodeURIComponent / decodeURIComponent
- **JSON 格式化** — 格式化 / 压缩

## 第三方依赖（无 CDN）

- **qrcodejs**：二维码生成使用本地库文件 `vendor/qrcode.min.js`（MIT License），许可证文本见 `vendor/licenses/qrcodejs-MIT.txt`。来源仓库为 `https://github.com/davidshimjs/qrcodejs`。

### 文本处理

- **正则测试** — pattern + flags 匹配与结果列表
- **字数统计** — 字符/单词/行数/字节统计

### 时间与数字

- **时间戳转换** — 秒/毫秒与本地时间互转
- **进制转换** — 二/八/十/十六进制（BigInt）

## 后续可扩展

编解码、文本处理、时间与数字等分类还可以继续补充更多工具（如大小写转换、Markdown 预览、Diff 对比等）。

## 部署到 Vercel

1. 将本仓库推送到 GitHub
2. 在 [Vercel](https://vercel.com) 导入该仓库
3. 保持默认设置（无构建命令，根目录即静态根）
4. 部署完成后即可通过生成的域名访问
