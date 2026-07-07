# 韩晨龙 · 个人作品集

纯静态单页站点(HTML / CSS / JS,无构建步骤),用于展示前端经历与作品。

## 本地预览

直接双击 `index.html`,或:

```bash
npx serve
```

## 部署到 Vercel(自定义域名 + 自动 HTTPS)

1. 在 GitHub 新建仓库,例如 `portfolio`(归属 `HCLacids`)。
2. 本地推送本仓库:

   ```bash
   git remote add origin git@github.com:HCLacids/portfolio.git
   git branch -M main
   git push -u origin main
   ```

3. 打开 [vercel.com](https://vercel.com) → **Add New → Project** → 导入刚才的仓库。
   Framework 选 **Other**,其余默认,点 **Deploy**。
4. 部署成功后:Project → **Settings → Domains** → 添加你的域名(如 `hanchenlong.com`)。
   Vercel 会给出对应的 DNS 记录,去你的域名注册商后台填好即可:
   - 子域(如 `www.hanchenlong.com`):添加 **CNAME** 指向 `cname.vercel-dns.com`
   - 根域(如 `hanchenlong.com`):按提示添加 **A 记录**(通常 `76.76.21.21`)
   等几分钟生效,HTTPS 证书自动签发。
5. 之后改了内容,推上去就自动重新部署:

   ```bash
   git add index.html && git commit -m "update" && git push
   ```

## 备注

- `.workbuddy/` 与 `dist/` 已加入 `.gitignore`,不会进仓库(私人记录不外传)。
- 自定义域名购买建议(`.com` / `.dev` / `.me` 等)见对话记录。
- 当前 CloudStudio 沙箱临时地址(仍可用):
  https://de4a8107867e4ae2820aba4924dbab6f.app.codebuddy.work
