# 拾蔚网络科技 · 产品官网

班级怪兽牧场产品官网（静态单页）。主体：**拾蔚网络科技有限公司**（AI 干货的一人公司）。

## 位置

- 静态文件目录：`~/桌面/shiwei-website/`
- 主页面：`index.html`（单页长滚动，文案/样式全在此文件）
- 素材：`assets/pets/`（真实精灵立绘、皮肤、海报）

## 访问

- 本地：http://localhost:8090
- GitHub 仓库：https://github.com/TheMrxk/shiwei-website
- 线上（GitHub Pages）：https://blog.orghub.cn/shiwei-website/

## 本地运行（Docker，端口 8090）

```bash
docker compose up -d --build
```

## 更新内容

```bash
# 改完 index.html 后
git add .
git commit -m "更新官网"
git push
```

push 到 main 后 GitHub Pages 自动构建更新。

## 定价

月卡 ¥29 / 季卡 ¥79 / 年卡 ¥289（在 index.html 价格区，直接改数字即可）。

## 关于域名

当前生效自定义域名是 `blog.orghub.cn`（配置在 TheMrxk.github.io 仓库的 CNAME 中）。

若日后改用 `10v.cc`：
1. Cloudflare DNS：加 CNAME 指向 `themrxk.github.io`（根域名可用 A 记录指向 GitHub Pages 的 185.199.108~111.153）
2. GitHub：对应仓库放/改 `CNAME` 文件为新域名
3. 等 GitHub 自动签发 HTTPS 证书（Settings → Pages 可看状态）
