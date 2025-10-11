# Repository Structure | 仓库结构

[English](#english) | [中文](#中文)

## English

### Directory Organization

This repository uses a category-based organization system for storing book files.

#### Category Descriptions

- **fiction/** - Fiction books including novels, short stories, and literary fiction
- **non-fiction/** - Non-fiction books including biographies, history, self-help, etc.
- **technical/** - Technical books, programming manuals, software documentation
- **academic/** - Academic papers, research publications, textbooks
- **magazines/** - Magazines, periodicals, journals
- **comics/** - Comics, manga, graphic novels

### Subcategories

You can create subcategories within each main category as needed. For example:

```
books/
├── technical/
│   ├── programming/
│   ├── databases/
│   └── web-development/
├── fiction/
│   ├── science-fiction/
│   ├── fantasy/
│   └── mystery/
```

### File Organization Best Practices

1. **Consistent naming**: Always use the format `[Author]_[Title]_[Year].[ext]`
2. **Avoid special characters**: Use underscores instead of spaces
3. **Use descriptive names**: Make filenames searchable and meaningful
4. **Include edition info**: For multiple editions, add edition number: `Author_Title_2024_2nd_Edition.pdf`

### Integration with E-Library

The main E-Library project will:
1. Index files from this repository
2. Maintain metadata (author, title, ISBN, description, etc.)
3. Provide search and discovery features
4. Link to files stored here

---

## 中文

### 目录组织

本仓库使用基于分类的组织系统来存储图书文件。

#### 分类说明

- **fiction/** - 小说类图书，包括长篇小说、短篇小说和文学作品
- **non-fiction/** - 非小说类图书，包括传记、历史、自助等
- **technical/** - 技术类书籍、编程手册、软件文档
- **academic/** - 学术论文、研究出版物、教科书
- **magazines/** - 杂志、期刊、学刊
- **comics/** - 漫画、图像小说

### 子分类

您可以根据需要在每个主分类中创建子分类。例如：

```
books/
├── technical/
│   ├── programming/
│   ├── databases/
│   └── web-development/
├── fiction/
│   ├── science-fiction/
│   ├── fantasy/
│   └── mystery/
```

### 文件组织最佳实践

1. **统一命名**：始终使用格式 `[作者]_[书名]_[年份].[扩展名]`
2. **避免特殊字符**：使用下划线代替空格
3. **使用描述性名称**：使文件名可搜索且有意义
4. **包含版本信息**：对于多个版本，添加版本号：`作者_书名_2024_第2版.pdf`

### 与E-Library集成

主E-Library项目将：
1. 索引此仓库中的文件
2. 维护元数据（作者、标题、ISBN、描述等）
3. 提供搜索和发现功能
4. 链接到此处存储的文件
