# 读书笔记 · 指令生成器

网站链接🔗：https://jianan-huang0609.github.io/KnowVis/

单文件网页工具：上传**文件名** / 粘贴**文字** / 添加**链接** → 一键生成可直接交给任意 AI 的完整 Prompt，返回**系统化读书笔记 + 单文件 HTML 网站源码**。

## 亮点
- **Bento Grid** 视觉：白底 + 自定义主题色（默认 `#F05E1C`）
- **单文件部署**：`index.html` 直接丢到 GitHub Pages 即可
- **一键 Prompt**：内置你要求的 14 条设计/技术规范（Tailwind 3、Framer Motion/回退方案、图标库、SVG 勾线图、滚动动效、导出 HTML 按钮等）
- **不读取隐私内容**：本工具不解析文件内容，只把**文件名**汇总进 Prompt 的 DOC_LIST，真正解析在 AI 端进行

## 使用方法
1. 下载本仓库或仅下载 `index.html`。
2. 打开浏览器访问本地文件（双击或拖到浏览器）即可使用。
3. 在页面内：
   - 选择主题色（或保持默认 `#F05E1C`）。
   - 填写标题、输出文件名、语言配比、可选图表库。
   - 上传文件（只会读取文件名）、粘贴文本、添加链接（每行一个）。
   - 点击 **“生成指令”**，随后可 **复制** 或 **下载为 .txt**。
4. 将生成的 Prompt 发送给你常用的 AI，得到：
   - **A. 系统化读书笔记（Markdown）**
   - **B. 单文件 HTML 源码**（含 Bento + 动效 + 图表占位 + 导出按钮）
5. 若要把 AI 生成的 HTML 上线：
   - 将其保存为 `index.html`；
   - 推送到 GitHub 仓库并开启 **GitHub Pages**（`Settings` → `Pages`）。

## GitHub Pages 快速发布
- 建议仓库结构：
  ```
  your-repo/
  ├─ index.html     # 本工具页面（指令生成器）
  └─ README.md
  ```
- 在仓库设置中启用 GitHub Pages，分支选择 `main`，目录选 `/root`。
- 等待生效后，访问 `https://<your-user>.github.io/<your-repo>/` 即可在线使用。

## 自定义
- 可在页面右上角使用 **导出按钮** 将生成的 Prompt 另存为 `.txt`。
- 若需更换默认主题色，请编辑 `index.html` 顶部 `:root{ --primary:#F05E1C; }`。

## 许可
MIT
