## Welcome to Lwming Pages

陪伴大憨憨小邓菌学习的一天开始了！

### B树和B+树的异同

今天来简单复习一下B树和B+树。B+树是所有信息都绑定到叶子节点上，然后叶子节点上彼此之间有一个指针指向对方。这样做的好处就是我拿出一个index出来做检索，可以很方便的检索，而不是像B树那样每一个叶子节点都是独立的，要回溯访问。

### 集簇和非集簇

首先要明确一点，集簇和非集簇，都是针对B+树来说的哟。因为B树这东东叶子之间没有指针，太拉了，大家表示无福消受。集簇就是所有表格信息都集中到了叶子节点上头，而非集簇则是叶子节点上只有信息的地址信息。只存地址信息的好处就是，由索引建立的B+树短小精悍，缺点就是查询的速度慢。因为我每次只能拿到一个地址，这个地址是什么呢，我又要去按图索骥，找找硬盘内存问问看，浪费时间了撒。于是集簇出现了，那么它就把信息都给绑定到了叶子上，这样查询的速度自然是快起来了。缺点就是索引的树存储大一些。



You can use the [editor on GitHub](https://github.com/459548764/homepage/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/459548764/homepage/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
