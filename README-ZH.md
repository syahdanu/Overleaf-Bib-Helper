# Overleaf-Bib-Helper

一个增强 Overleaf 的 UserScript，可在 Overleaf 编辑器中直接从 DBLP 和 Google Scholar 搜索文章并获取 BibTeX。

- **GitHub 仓库**: [https://github.com/Arvid-pku/Overleaf-Bib-Helper](https://github.com/Arvid-pku/Overleaf-Bib-Helper)
- **Greasy Fork 页面**: [https://greasyfork.org/zh-CN/scripts/532304-overleaf-bib-helper](https://greasyfork.org/zh-CN/scripts/532304-overleaf-bib-helper)

## 功能
- 在 Overleaf 中从 DBLP 或 Google Scholar 搜索学术文章。
- 一键获取并复制 BibTeX 条目。
- 可配置的结果数量（5、10、20 或 50 个结果）。
- 可滚动的搜索结果列表，便于浏览。
- 键盘快捷键：Enter 键搜索，Esc 键关闭弹窗。
- 支持多个 Google Scholar 镜像以提高访问性。

## 安装

### 第一步：安装 Tampermonkey
Tampermonkey 是一个浏览器扩展，用于运行 UserScript，例如 Overleaf-Bib-Helper。请按照以下步骤操作：

1. **下载 Tampermonkey**：
   - **Chrome**: 从 [Chrome 网上应用店](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) 安装。
   - **Firefox**: 从 [Mozilla 附加组件](https://addons.mozilla.org/zh-CN/firefox/addon/tampermonkey/) 安装。
   - **Edge**: 从 [Microsoft Edge 扩展](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmleipfamncoeapigifbpdccjedebe) 安装。
   - **Safari**: 从 [App Store](https://apps.apple.com/cn/app/tampermonkey/id1482490089) 安装（需要 macOS）。

2. **启用 Tampermonkey**：
   - 安装完成后，点击浏览器工具栏中的 Tampermonkey 图标，确保其已启用。

### 第二步：安装 Overleaf-Bib-Helper
您可以通过以下两种方式安装脚本：

#### 选项 1：从 Greasy Fork 安装（推荐）
1. 访问 [Greasy Fork 页面](https://greasyfork.org/zh-CN/scripts/532304-overleaf-bib-helper)。
2. 点击 **“安装此脚本”** 按钮。
3. Tampermonkey 将打开一个确认窗口，点击 **“安装”** 添加脚本。
4. 脚本将在 Overleaf 项目页面（`https://www.overleaf.com/project/*`）上自动激活。

#### 选项 2：从 GitHub 安装
1. 前往 [GitHub 仓库](https://github.com/Arvid-pku/Overleaf-Bib-Helper)。
2. 打开仓库中的 `Overleaf-Bib-Helper.js` 文件。
3. 复制整个脚本内容。
4. 在浏览器中，点击 Tampermonkey 图标 > **“创建新脚本”**。
5. 将复制的代码粘贴到编辑器中，替换默认模板。
6. 点击 **文件 > 保存**。
7. 脚本将在 Overleaf 项目页面上激活。

## 使用方法

### 打开工具
1. 在浏览器中打开一个 Overleaf 项目（`https://www.overleaf.com/project/*`）。
2. 在 Overleaf 工具栏中查找新图标（一个类似文档的小图标）。
3. 点击图标以打开搜索弹窗。

### 搜索文章
1. **输入查询**：在输入框中输入搜索词（如文章标题、作者或关键词）。
2. **选择来源**：从“来源”下拉菜单中选择“DBLP”或“Google Scholar”。
3. **设置结果数量**：从“结果”下拉菜单中选择 5、10、20 或 50 个结果。
4. **开始搜索**：
   - 按下 **Enter** 键，或
   - 点击输入框旁边的放大镜图标。
5. 搜索结果将显示在输入框下方的可滚动列表中。如果结果较多，可滚动浏览。

### 复制 BibTeX
1. 点击列表中的任何结果（例如“标题@作者”）。
2. BibTeX 条目将被复制到剪贴板。
3. 将显示通知，确认复制成功（“复制成功”）或报告错误（“复制失败”）。

### 关闭弹窗
- 在弹窗打开时，随时按下 **Esc** 键关闭弹窗，或
- 再次点击工具栏图标以切换关闭弹窗。

## 键盘快捷键
- **Enter**: 从输入框触发搜索。
- **Esc**: 在页面任何位置关闭弹窗。

## 注意事项
- **Google Scholar**：偶尔可能需要验证码验证。如果 BibTeX 获取失败，脚本将打开 Google Scholar 页面以供手动操作。
- **偏好设置**：您选择的来源和结果数量将在会话间保存。
- **兼容性**：仅在 Overleaf 项目页面上生效。请确保您位于项目 URL（`https://www.overleaf.com/project/*`）。

## 故障排除
- **脚本不起作用？**
  - 确保 Tampermonkey 已启用且脚本处于活动状态（检查 Tampermonkey 仪表盘）。
  - 确认您在 Overleaf 项目页面上。
  - 刷新页面或从 Greasy Fork 重新安装脚本。
- **没有搜索结果？**
  - 检查搜索查询是否有拼写错误。
  - 尝试在 DBLP 和 Google Scholar 之间切换，因为它们的覆盖范围不同。
- **Google Scholar 问题？**
  - 如果遇到验证码阻碍，请在打开的标签页中完成验证后重试。

## 贡献
欢迎 fork [GitHub 仓库](https://github.com/Arvid-pku/Overleaf-Bib-Helper)，提交问题或通过拉取请求提供改进建议！
