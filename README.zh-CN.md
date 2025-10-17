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
