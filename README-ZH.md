<div align="center">
  <img src="figure/logo.png" width="50" />
  <h1>Overleaf-Bib-Helper</h1>
</div>

<p align="center">
  一个用户脚本，用于增强 Overleaf 功能，支持在 Overleaf 编辑器中直接从 DBLP 和 Google Scholar 搜索文章并获取 BibTeX 条目。
</p>

<p align="center">
  <a href="https://greasyfork.org/zh-CN/scripts/532304-overleaf-bib-helper">
    <img alt="从 Greasy Fork 安装" src="https://img.shields.io/badge/Install-Greasy_Fork-blue" />
  </a>
  <a href="https://github.com/MLNLP-World/Overleaf-Bib-Helper/releases">
    <img alt="版本" src="https://img.shields.io/badge/Version-1.2-blue" />
  </a>
  <a href="https://github.com/MLNLP-World/Overleaf-Bib-Helper/blob/main/LICENSE.md">
    <img alt="许可证" src="https://img.shields.io/badge/License-MIT-blue" />
  </a>
  <a href="https://github.com/MLNLP-World/Overleaf-Bib-Helper/stargazers">
    <img alt="Stars" src="https://img.shields.io/github/stars/MLNLP-World/Overleaf-Bib-Helper" />
  </a>
  <a href="https://github.com/MLNLP-World/Overleaf-Bib-Helper/network/members">
    <img alt="Forks" src="https://img.shields.io/github/forks/MLNLP-World/Overleaf-Bib-Helper" />
  </a>
  <a href="https://github.com/MLNLP-World/Overleaf-Bib-Helper/issues">
    <img alt="Issues" src="https://img.shields.io/github/issues/MLNLP-World/Overleaf-Bib-Helper" />
  </a>
  <a href="https://github.com/MLNLP-World/Overleaf-Bib-Helper/pulls">
    <img alt="欢迎 PR" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" />
  </a>
</p>

---

<div>
<p align="center">
      <a href="README-ZH.md">中文文档</a> •
      <a href="#安装">安装</a> •
      <a href="#使用方法">使用方法</a> •
      <a href="#支持的来源">支持的来源</a> •
      <a href="#故障排除">故障排除</a> •
      <a href="#免责声明">免责声明</a> •
      <a href="#更新日志">更新日志</a> •
      <a href="#许可证">许可证</a> •
      <a href="#贡献">贡献</a> •
      <a href="#联系方式">联系方式</a> •
      <a href="#组织者">组织者</a> •
      <a href="#贡献者">贡献者</a> •
      <a href="#致谢">致谢</a>
    </p>
</div>

## 动机
撰写 LaTeX 文档时通常需要包含大量学术参考文献。手动搜索和格式化 BibTeX 条目非常耗时。Overleaf-Bib-Helper 通过将 DBLP 和 Google Scholar 的搜索功能集成到 Overleaf 界面中，简化了这一过程，使用户能够快速查找和复制 BibTeX 条目，省时省力。

## 功能
- 在 Overleaf 中搜索 DBLP 或 Google Scholar 的学术文章。
- 一键获取并复制 BibTeX 条目。
- 可配置的结果数量（5、10、20 或 50 个结果）。
- 可滚动的搜索结果列表，便于浏览。
- 键盘快捷键：回车键搜索，Esc 键关闭弹出窗口。
- 支持多个 Google Scholar 镜像以提高访问性。

## 更新日志
- **2025-04-14**：新增 Google Scholar 高级搜索选项支持（v1.3）。
- **2025-04-10**：新增对 cn.overleaf.com 和 cn.overleaf.com 域名的支持（v1.2）。
- **2025-04-09**：初始版本，包含 DBLP 和 Google Scholar 的基本功能（v1.1）。

## 安装
### 步骤 1：安装 Tampermonkey
Tampermonkey 是一个运行用户脚本（如 Overleaf-Bib-Helper）所需的浏览器扩展。请按照以下步骤操作：
1. **下载 Tampermonkey**：
   - **Chrome**：[Chrome 网上应用店](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
   - **Firefox**：[Mozilla 附加组件](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
   - **Edge**：[Microsoft Edge 附加组件](https://microsoftedge.microsoft.com/addons/detail/%E7%AF%A1%E6%94%B9%E7%8C%B4/iikmkjmpaadaobahmlepeloendndfphd)
   - **Safari**：[App Store](https://apps.apple.com/us/app/tampermonkey/id1482490089)（需要 macOS）
2. **启用 Tampermonkey**：
   - 安装完成后，点击浏览器工具栏中的 Tampermonkey 图标，确保其已启用。
3. **启用扩展的开发者模式**：
   - 对于 Chrome，前往扩展页面（`chrome://extensions/`）并启用开发者模式。

### 步骤 2：安装 Overleaf-Bib-Helper
您可以通过以下两种方式安装脚本：

#### 选项 1：从 Greasy Fork 安装（推荐）
1. 访问 [Greasy Fork 页面](https://greasyfork.org/zh-CN/scripts/532304-overleaf-bib-helper)。
2. 点击 **“安装此脚本”** 按钮。
3. Tampermonkey 将打开一个确认窗口，点击 **“安装”** 添加脚本。
4. 脚本将在 Overleaf 项目页面（`https://www.overleaf.com/project/*`）自动激活。
5. 为保持脚本更新，请在 Tampermonkey 设置中启用自动更新。

#### 选项 2：从 GitHub 安装
1. 前往 [GitHub 仓库](https://github.com/MLNLP-World/Overleaf-Bib-Helper)。
2. 打开仓库中的 `Overleaf-Bib-Helper.js` 文件。
3. 复制整个脚本内容。
4. 在浏览器中，点击 Tampermonkey 图标 > **“创建新脚本”**。
5. 将复制的代码粘贴到编辑器中，替换默认模板。
6. 在 Tampermonkey 编辑器中点击 **文件 > 保存**。
7. 脚本将在 Overleaf 项目页面上激活。
8. **注意**：从 GitHub 手动安装时，请定期检查仓库更新并重新安装。

## 使用方法
### 打开工具
1. 在浏览器中打开一个 Overleaf 项目（`https://www.overleaf.com/project/*`）。
2. 在 Overleaf 工具栏中查找新图标（一个类似文档的小图标）。
3. 点击图标打开搜索弹出窗口。

<div align="center">
<img src="figure/instruction.jpg" width="180" />
</div>

### 搜索文章
1. **输入查询**：在输入框中键入搜索词（例如文章标题、作者或关键词）。
2. **选择来源**：从“来源”下拉菜单中选择“DBLP”或“Google Scholar”。
   - **DBLP**：适合计算机科学文献，数据结构化。
   - **Google Scholar**：覆盖更广泛的学科，但可能需要 CAPTCHA 验证。
3. **设置结果数量**：从“结果”下拉菜单选择 5、10、20 或 50 个结果。
4. **开始搜索**：
   - 按 **回车键** 或点击放大镜图标。
5. 搜索结果将显示在输入框下方的可滚动列表中。

### 复制 BibTeX
1. 点击列表中的任一结果（例如“标题@作者”）。
2. BibTeX 条目将复制到剪贴板。
3. 将显示通知确认成功（“复制成功”）或报告错误（“复制失败”）。

<div align="center">
<img src="figure/result.png" width="280" />
</div>

### 关闭弹出窗口
- 按 **Esc 键** 或再次点击工具栏图标。

## 支持的来源
- **DBLP**：计算机科学领域的综合文献数据库，提供可靠的 BibTeX 条目。
- **Google Scholar**：覆盖更广泛的学术搜索引擎，可能包含更近期或跨学科的内容，但可能需要用户验证（例如 CAPTCHA）。

## 故障排除
- **脚本不起作用？**
  - 确保浏览器已为扩展启用 **开发者模式**。
  - 确保 Tampermonkey 已启用且脚本处于激活状态。
  - 确认您在 Overleaf 项目页面上。
  - 尝试从 Greasy Fork 重新加载或重新安装。
- **没有结果？**
  - 检查查询是否有拼写错误。
  - 确保已授予插件搜索权限。
  - 尝试在 DBLP 和 Google Scholar 之间切换。
- **Google Scholar 问题？**
  - 如果 CAPTCHA 阻止访问，请在打开的标签页中完成验证并重试。

## 免责声明
尽管 Overleaf-Bib-Helper 旨在提供无缝体验，但请注意，它依赖外部服务（DBLP 和 Google Scholar），这些服务的 API 可能发生变化或需要用户验证（例如 CAPTCHA）。请谨慎使用此工具，并在将检索的 BibTeX 条目纳入文档前始终进行验证。

## 许可证
本项目采用 MIT 许可证，详情见 [LICENSE.md](https://github.com/MLNLP-World/Overleaf-Bib-Helper/blob/main/LICENSE.md)。

## 贡献
欢迎 fork [GitHub 仓库](https://github.com/MLNLP-World/Overleaf-Bib-Helper)，提交问题或通过拉取请求提出改进！

## 联系方式
如有任何问题或建议，请发送邮件至 [Xunjian Yin](mailto:xjyin@pku.edu.cn) 或在此处创建 GitHub 问题。

## 组织者
<a href="https://github.com/Arvid-pku">  <img src="https://avatars.githubusercontent.com/u/53811705?s=96&v=4"  width="55" > </a> 

## 贡献者
<a href="https://github.com/Arvid-pku">  <img src="https://avatars.githubusercontent.com/u/53811705?s=96&v=4"  width="55" > </a> 
<a href="https://github.com/QAbot-zh">  <img src="https://avatars.githubusercontent.com/u/40236765?v=4"  width="55" > </a> 

## 致谢
受类似工具和学术界对高效参考管理的启发。