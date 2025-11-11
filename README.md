# Vercel Redirect

一个基于 Vercel 的简单域名重定向服务。

## 功能特点

- ✅ 301 永久重定向
- ✅ 路径参数保留
- ✅ 免费部署
- ✅ 全球 CDN 加速

## 快速开始

1. Fork 本项目
2. 修改 `vercel.json` 中的目标 URL
3. 在 Vercel 中导入项目
4. 配置自定义域名

## 配置

```json
{
  "redirects": [
    {
      "source": "/",
      "destination": "https://目标网站.com",
      "permanent": true
    },
    {
      "source": "/(.*)",
      "destination": "https://目标网站.com/:1",
      "permanent": true
    }
  ]
}
```