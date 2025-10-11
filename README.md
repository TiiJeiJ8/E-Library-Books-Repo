# E-Library-Books-Repo

[EN English](./README.md) | [ZH 中文](./README.zh-CN.md)

This folder is the canonical location for storing actual e-book files (PDF/EPUB/MOBI/AZW, etc.).

- The `books/` folder in the main [**E-Library**](https://github.com/TiiJeiJ8/E-Library/README.md) repository is used only as an index/catalog (views by author / category / topic).

- Place all binary book files under `library/` using clear subfolders (e.g., Author/Title/Year or similar).

- Documentation (summaries and reading notes) is stored in the main [**E-Library**](https://github.com/TiiJeiJ8/E-Library/README.md) repository's `docs/` directory and is linked to the corresponding entries from the `books/` index pages.

## Suggested Structure

```
library/
  Author-Last-Name-First-Name/
    Book-Title-YYYY/
      AuthorLastName_BookTitle_Year.cn.pdf
      AuthorLastName_BookTitle_Year.en.epub
      AuthorLastName_BookTitle_YYYY.<language>.ext
```

## Notes

- Do not commit copyrighted materials unless they are public domain, under open licenses, or you have explicit permission.
- Keep filenames descriptive and consistent with the naming convention.
