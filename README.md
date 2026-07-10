# FOMO Colour Gallery — 部署说明

这个文件夹是**干净的可发布版本**,只含 `index.html` + 展示用的真车实拍图。
**不含任何 TeckWrap 文件**(无 manifest、无卷材图、无水印),可安全发布到公开的 GitHub 仓库。

- 颜色数：172
- 图片数：1367（原画质，未压缩）
- 体积：约 189 MB

---

## 用 GitHub Pages 上线（推荐命令行）

1. 在 https://github.com/new 建一个**公开(Public)** 仓库，例如 `fomo-colours`（先不要勾选 Add README）。

2. 打开终端(PowerShell)，进入本文件夹并推送：

```bash
cd "C:\Users\Aufb\OneDrive - FOMO AUTO CUSTOMS STUDIO\FOMO\marketing\TeckWrap官网产品图\fomo-colour-site"
git init
git add .
git commit -m "FOMO colour gallery"
git branch -M main
git remote add origin https://github.com/<你的用户名>/fomo-colours.git
git push -u origin main
```

3. 仓库页面 → **Settings → Pages** → Source 选 **Deploy from a branch** → 分支选 `main`、目录选 `/ (root)` → **Save**。

4. 等 1–2 分钟，页面顶部会出现网址：

```
https://<你的用户名>.github.io/fomo-colours/
```

5. 把这个网址发给我 → 我立刻生成**二维码图片**给你印刷（名片 / 门店 / 报价单）。

---

## 不想用命令行？（网页上传）

在新建的空仓库页面点 **“uploading an existing file”**，把本文件夹里的所有内容拖进去提交。
注意：文件多(1300+)，网页上传可能要分几次、较慢；命令行 `git push` 更稳。

---

## 更新颜色 / 图片后

重新生成本文件夹后，再次：

```bash
git add .
git commit -m "update"
git push
```

Pages 会自动重新发布。
