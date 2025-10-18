# E-Library-Books-Repo

[EN English](./README.md) | [ZH 中文](./README.zh-CN.md)

This folder is the canonical location for storing actual e-book files (PDF/EPUB/MOBI/AZW, etc.).

- The `books/` folder in the main [**E-Library**](https://github.com/TiiJeiJ8/E-Library/blob/main/README.md) repository is used only as an index/catalog (views by author / category / topic).

- Place all binary book files under `library/` using clear subfolders (e.g., Author/Title/Year or similar).

- Documentation (summaries and reading notes) is stored in the main [**E-Library**](https://github.com/TiiJeiJ8/E-Library/blob/main/README.md) repository's `docs/` directory and is linked to the corresponding entries from the `books/` index pages.

## Suggested Structure

```
library/
  Author-Last-Name-First-Name/
    Book-Title-YYYY/
      AuthorLastName_BookTitle_Year.cn.pdf
      AuthorLastName_BookTitle_Year.en.epub
      AuthorLastName_BookTitle_YYYY.<language>.ext
```
If a file is too large to upload directly via the web, you can try splitting it into multiple parts (we recommend using the [tool](https://github.com/TiiJeiJ8/LibSpliter) we created), and name them according to the following structure:
```
library/
  Author-Last-Name-First-Name/
    Book-Title-YYYY/
      AuthorLastName_BookTitle_Year-1.cn.pdf
      AuthorLastName_BookTitle_Year-2.cn.pdf
      AuthorLastName_BookTitle_Year-3.cn.pdf
      AuthorLastName_BookTitle_YYYY.<language>-part.ext
```

## Notes

- Do not commit copyrighted materials unless they are public domain, under open licenses, or you have explicit permission.
- Keep filenames descriptive and consistent with the naming convention.

### CI checks

A GitHub Actions workflow (`.github/workflows/PR_Check.yml`) automatically validates filenames and paths under the repository's `library/` directory on pushes and pull requests that touch `library/**`. The check enforces the repository's naming conventions (expected folder depth, allowed file extensions, and a filename pattern that includes a four‑digit year). If the check fails, the action will mark the run as failed and print which files didn't match.

If you believe a file was flagged in error or need an exception (for special characters, different naming, or large split files), please open an issue or submit a small follow-up commit to rename the files. If you want the maintainers to relax or change the filename rules, describe which characters or patterns to allow and the workflow can be updated.

How to test locally / in a PR

- Create a branch, add or modify one file under `library/`, push and open a pull request targeting `main`.
- The GitHub Actions run will appear on the PR page; failing step output shows which file(s) violated the rules.
