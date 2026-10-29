Our Money 第一版：本地试用 PWA

文件：index.html、manifest.webmanifest、icon.svg、sw.js

使用方法：
1. 电脑上可直接打开 index.html 试用（本地文件方式不启用 PWA 安装）。
2. 要在 iPhone 上作为 PWA 安装：将整个文件夹部署到 HTTPS 静态网站托管服务（如 GitHub Pages / Netlify），Safari 打开网站，分享 > 添加到主屏幕。
3. 当前交易数据仅储存在每台设备自己的 localStorage。不会跨手机同步，也没有用户登录。请定期导出 JSON 备份。
4. 下一版实现夫妻同步需要数据库和登录系统（例如 Supabase），必须配置访问控制，绝不能把 service_role 密钥放在网页代码中。
