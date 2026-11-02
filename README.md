# 悦读书阁 v2

全新暗红黑金主题，无首页顶部大 Banner。原生 HTML/CSS/JavaScript/JSON，可直接部署 GitHub Pages。

## 页面和功能
- 首页直接进入分类、编辑精选与作品书库
- 20 部虚构示例作品，包含较完整的简介、作者、分类、标签、状态
- 11 类小说题材
- 每部作品独立 HTML 详情页（含静态首屏内容，便于爬虫读取）
- 分类筛选、关键词搜索、本地收藏、明暗主题
- 4 个友情链接、移动端适配、robots.txt、sitemap.xml

## 本地预览
在项目根目录运行 `python -m http.server 8000`，打开 http://localhost:8000 。

## GitHub Pages 部署
1. 新建 GitHub Public 仓库。
2. 上传本目录内所有文件至仓库根目录。
3. 仓库 Settings → Pages → Deploy from a branch。
4. Branch 选择 main，目录选择 /(root)，保存。
5. 发布后访问 `https://你的用户名.github.io/仓库名/`。

## 上线前必须修改
- 全局替换 `YOUR_GITHUB_USERNAME` 和 `YOUR_REPOSITORY`，更新 HTML canonical、robots.txt、sitemap.xml。
- 在 data.json 修改小说、作者、分类、简介、封面、友链。
- 新增作品时，在 books/ 目录创建独立详情页，并在 data.json 添加相同 id。
- 示例封面来自 Unsplash 外链。正式使用前请确认图片许可、可用性；也可以换成自有或获得授权的成年模特/人物摄影，并放入 assets/covers/ 后使用相对路径。

## 说明
本站是静态作品介绍和发现站，不含账号、后台、章节数据库或全文阅读。收藏只保存在当前浏览器。作品示例均为虚构内容。成人文学仅限合法合规的成年题材，不得涉及未成年人性化内容或违法内容。友情链接上线前请核实合作关系及链接准确性。
