# 手机网页部署说明

这个目录是可直接发布的静态 H5 手机网页。

入口文件：

```text
index.html
```

## 本地预览

在项目根目录运行：

```bash
python -m http.server 8080 -d public_mobile
```

然后打开：

```text
http://localhost:8080
```

手机在同一个 Wi-Fi 下访问时，把 `localhost` 换成电脑的局域网 IP。

## 部署到线上

可以任选一个静态托管平台：

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages

上传 `public_mobile` 目录即可。部署完成后，别人打开平台生成的网址就能直接使用。

## 说明

- 手机打开时会自动变成全屏 App 页面。
- 电脑打开时会保留 iPhone 预览壳，适合作品集展示。
- 这个静态网页不依赖 Python 后端，适合发链接给别人体验。
