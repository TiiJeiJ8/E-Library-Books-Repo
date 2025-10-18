# E-Library 书库（E-Library-Books-Repo）

[EN English](./README.md) | [ZH 中文](./README.zh-CN.md)

此文件夹用于存放实际的电子书文件（PDF/EPUB/MOBI/AZW 等）。

- 主仓库 [**E-Library**](https://github.com/TiiJeiJ8/E-Library/blob/main/README.zh-CN.md) 中的 `books/` 仅作为索引/目录视图（按作者/类别/主题）。
- 请将所有二进制书籍文件放在本仓库的 `library/` 下，并使用清晰的子目录结构（如 作者/书名/年份）。
- 文档（摘要、阅读笔记）存放在主仓库 [**E-Library**](https://github.com/TiiJeiJ8/E-Library/blob/main/README.zh-CN.md) 中的 `docs/`，并由 `books/` 索引页面链接到相应条目。

## 推荐结构

```
library/
  Author-Last-Name-First-Name/
    Book-Title-YYYY/
      AuthorLastName_BookTitle_Year.cn.pdf
      AuthorLastName_BookTitle_Year.en.epub
      AuthorLastName_BookTitle_YYYY.<language>.ext
```
如果有文件过大无法直接通过网页上传，可以尝试将文件拆分为多块 ( 推荐使用我制作的[小工具](https://github.com/TiiJeiJ8/LibSpliter) )，按如下结构命名
```
library/
  Author-Last-Name-First-Name/
    Book-Title-YYYY/
      AuthorLastName_BookTitle_Year-1.cn.pdf
      AuthorLastName_BookTitle_Year-2.cn.pdf
      AuthorLastName_BookTitle_Year-3.cn.pdf
      AuthorLastName_BookTitle_YYYY.<language>-part.ext
```

## 注意

- 不要提交受版权保护且无授权的内容；仅提交公有领域、开源许可或已获明确授权的资料。
- 请遵循命名规范并保持一致性。

### CI 检查

仓库已启用一个 GitHub Actions 工作流（位于 `.github/workflows/PR_Check.yml`），在 push 或涉及 `library/**` 的 Pull Request 时自动校验 `library/` 下的路径与文件名是否符合命名规范（目录层级、允许的文件扩展名以及包含四位年份的文件名模式）。若检查失败，Action 会将运行标记为失败并输出不符合规则的文件信息。

如果你认为某个文件被误判，或需要为特殊字符/命名/分片文件设置例外，请打开 issue 或提交一个小的修正提交来重命名文件。如果你希望维护者放宽或修改校验规则，请描述希望允许的字符或模式，工作流随后可以更新。

如何测试

- 本地创建一个分支，在 `library/` 下添加或修改文件，push 后创建针对 `main` 的 PR。
- 在 PR 页面查看 Actions 运行结果，失败步骤会显示具体不合规的文件。
