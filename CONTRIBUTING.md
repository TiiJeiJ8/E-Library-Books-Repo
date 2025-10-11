# Contributing Guidelines | 贡献指南

[English](#english) | [中文](#中文)

## English

### How to Contribute

Thank you for considering contributing to the E-Library-Books-Repo! This repository stores book files that will be indexed by the main E-Library project.

### Before Adding Books

1. **Check for duplicates**: Ensure the book isn't already in the repository
2. **Verify file format**: Use commonly supported formats (PDF, EPUB, MOBI, AZW3, TXT)
3. **Respect copyright**: Only add books that are in the public domain or that you have permission to share
4. **File size**: Consider file size - keep files reasonable for version control

### Adding Books

1. **Choose the right category**: Place your book in the appropriate directory:
   - `books/fiction/` - Fiction books
   - `books/non-fiction/` - Non-fiction books
   - `books/technical/` - Technical books
   - `books/academic/` - Academic materials
   - `books/magazines/` - Magazines and periodicals
   - `books/comics/` - Comics and graphic novels

2. **Follow naming convention**: 
   ```
   [Author]_[Title]_[Year].[ext]
   ```
   Examples:
   - `John_Doe_The_Great_Novel_2023.pdf`
   - `Jane_Smith_Python_Programming_2024.epub`

3. **Create subdirectories if needed**: For better organization, you can create subcategories:
   ```
   books/technical/programming/Python_Developer_Guide.pdf
   ```

4. **Commit message format**:
   ```
   Add: [Book Title] by [Author]
   
   Category: [category name]
   Format: [file format]
   ```

### Pull Request Guidelines

1. One book per pull request (unless adding a series)
2. Provide a brief description of the book
3. Confirm copyright status
4. Ensure file naming follows conventions

### Legal Considerations

⚠️ **Important**: 
- Only add books that are legally distributable
- Public domain works are welcome
- If you have permission from the copyright holder, include documentation
- When in doubt, don't add the book

---

## 中文

### 如何贡献

感谢您考虑为E-Library-Books-Repo做出贡献！本仓库存储将由主E-Library项目索引的图书文件。

### 添加图书前

1. **检查重复**：确保仓库中尚未存在该图书
2. **验证文件格式**：使用常见支持的格式（PDF、EPUB、MOBI、AZW3、TXT）
3. **尊重版权**：仅添加公共领域的图书或您有权分享的图书
4. **文件大小**：考虑文件大小 - 保持文件大小适合版本控制

### 添加图书

1. **选择正确的分类**：将您的图书放在适当的目录中：
   - `books/fiction/` - 小说类图书
   - `books/non-fiction/` - 非小说类图书
   - `books/technical/` - 技术类书籍
   - `books/academic/` - 学术材料
   - `books/magazines/` - 杂志和期刊
   - `books/comics/` - 漫画

2. **遵循命名规范**：
   ```
   [作者]_[书名]_[年份].[扩展名]
   ```
   示例：
   - `张三_伟大的小说_2023.pdf`
   - `李四_Python编程_2024.epub`

3. **根据需要创建子目录**：为了更好地组织，您可以创建子分类：
   ```
   books/technical/programming/Python开发指南.pdf
   ```

4. **提交信息格式**：
   ```
   Add: [书名] by [作者]
   
   Category: [分类名称]
   Format: [文件格式]
   ```

### Pull Request指南

1. 每个pull request一本书（除非添加系列丛书）
2. 提供图书简要描述
3. 确认版权状态
4. 确保文件命名遵循规范

### 法律注意事项

⚠️ **重要**：
- 仅添加可合法分发的图书
- 欢迎公共领域作品
- 如果您获得版权持有者的许可，请附上文档
- 如有疑问，请勿添加该图书
