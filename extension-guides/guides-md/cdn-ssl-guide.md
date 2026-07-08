```json
{
  "id": "cdn-ssl-guide",
  "title": "Cloudflare CDN / SSL 配置建议",
  "description": "开启 Cloudflare CDN 后的 SSL/TLS 模式设置指引",
  "category": "cdn-setup",
  "vendorKey": "cloudflare",
  "tags": ["cloudflare", "cdn", "ssl", "tls"],
  "externalLinks": [
    { "label": "Cloudflare SSL/TLS 文档", "url": "https://developers.cloudflare.com/ssl/" }
  ]
}
```

## 步骤 1: 进入 SSL/TLS 设置
在 Cloudflare 控制台选择你的域名，左侧菜单点「SSL/TLS」→「Overview」。

## 步骤 2: 选择加密模式
将加密模式设为「Full (strict)」— 这是最安全的选项，要求源服务器有有效证书。

> [!tip] 推荐设置
> 如果你的源服务器使用 Let's Encrypt 或 Cloudflare Origin Certificate，选择「Full (strict)」。
> 如果源服务器使用自签名证书，可暂时选择「Full」，但建议尽快更换为正式证书。

## 步骤 3: 开启 Always Use HTTPS（可选）
在「SSL/TLS」→「Edge Certificates」中开启「Always Use HTTPS」，强制所有 HTTP 请求跳转到 HTTPS。

> [!info] 提示
> 开启后所有访客将自动通过 HTTPS 访问你的站点，无需在 WordPress 中额外配置。
