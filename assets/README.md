# 资源文件夹说明

这个文件夹专门放 `index.html` 用到的图片、图标一类的静态资源，跟页面代码分开管理。

## 目录结构

- `images/` — 照片、插画、截图等大图
- `icons/` — 小图标、logo、favicon 一类的小图

## 命名规范

- 一律用英文或拼音 + 短横线命名，例如 `logo-badge.png`、`empty-state.svg`
- 不要用中文、空格或大写开头，中文/空格文件名在网页地址里会被转成一长串 `%E5%9B...` 的编码，容易踩坑
- 名字要能看出用途，比如 `gate-icon.png` 比 `1.png` 好

## 怎么加新图片

1. 把图片文件放进 `assets/images/`（或 `assets/icons/`）
2. 在 `index.html` 里用相对路径引用，例如：
   ```html
   <img src="assets/images/xxx.png" alt="说明文字">
   ```
   或者在 CSS 里：
   ```css
   background-image: url('assets/icons/xxx.svg');
   ```
3. 在 GitHub Desktop 里能看到新增的图片文件和 `index.html` 的改动，一起 Commit + Push 即可

## 注意

- 这里只放你自己拥有版权、或者有合法使用授权的图片
- 官方角色原图、带版权水印的成品图这类内容不要放进来发布——这个仓库是公开可访问的网址，等于对外发布
