# 基本语法

## 1. 标题语法

# heading level 1

```markdown
# heading level 1
```

## heading level 2

```markdown
## heading level 2
```

### heading level 3

```markdown
### heading level 3
```

#### heading level 4

```markdown
#### heading level 4
```

##### heading level 5

```markdown
##### heading level 5
```

###### heading level 6

```markdown
###### heading level 6
```

## 2. 段落语法

I really like using Markdown.

I think I'll use it to format all of my documents from now on.

```markdown
I really like using Markdown.

I think I'll use it to format all of my documents from now on.
```

## 3. 换行语法

This is the first line.  
And this is the second line.

```markdown
This is the first line.  
And this is the second line.
```

## 4. 强调语法

### 4.1 斜体

Italicized text is the _cat's meow_.

```markdown
Italicized text is the _cat's meow_.
```

### 4.2 粗体

I just love **bold** text.

```markdown
I just love **bold** text.
```

### 4.3 粗体和斜体

This text is **_really important_**.

```markdown
This text is **_really important_**.
```

## 5. 引用语法

> Dorothy followed her through many of the beautiful rooms in her castle.

```markdown
> Dorothy followed her through many of the beautiful rooms in her castle.
```

### 5.1 多个段落的块引用

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fir

```markdown
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fir
```

### 5.2 嵌套块引用

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> > The Witch bade her clean the pots and kettles and sweep the floor and keep th

```markdown
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> > The Witch bade her clean the pots and kettles and sweep the floor and keep th
```

### 5.3 带其他元素的块引用

> ### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> _Everything_ is going according to **plan**.

```markdown
> ### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> _Everything_ is going according to **plan**.
```

## 6. 列表语法

### 6.1 有序列表

1. First item
2. Seconds item
3. Third item
4. Fourth item

```markdown
1. First item
2. Seconds item
3. Third item
4. Fourth item
```

### 6.2 无序列表

- First item
- Second item
- Third item
- Fourth item

```markdown
- First item
- Second item
- Third item
- Fourth item
```

### 6.3 在列表中嵌套其他元素

要保留列表的连续性的同时在列表中添加另一种元素， 请将该元素缩进四个空格或一个制表符

#### 6.3.1 段落

- This is the first list item.
- Here's the second list item.
  I need to add another paragraph below the second list item.
- And here's the third list item

```markdown
- This is the first list item.
- Here's the second list item.
  I need to add another paragraph below the second list item.
- And here's the third list item
```

#### 6.3.2 引用块

- This is the first list item.
- Here's the second list item.

  > A block quote would look great below the second list item.

- And here's the third list item.

```markdown
- This is the first list item.
- Here's the second list item.
  > A block quote would look great below the second list item.
- And here's the third list item.
```

#### 6.3.3 代码块

1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>
        </html>

3.  Update the title to match the name of your website.

```markdown
1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>
        </html>

3.  Update the title to match the name of your website.
```

#### 6.3.4 图片

1. Open the file containing the Linux mascot.
2. Marvel at the beauty.

   ![Tux, the linux mascot](../img/linux.png)

3. Close the file.

```markdown
1. Open the file containing the Linux mascot.
2. Marvel at the beauty.

   ![Tux, the linux mascot](../img/linux.png)

3. Close the file.
```

#### 6.3.5 列表

1. First item
2. Second item
3. Third item
   - Indented item
   - Indented item
4. Fourth item

```markdown
1. First item
2. Second item
3. Third item
   - Indented item
   - Indented item
4. Fourth item
```

## 7. 代码语法

At the command prompt, type `nano`.

```markdown
At the command prompt, type `nano`.
```

### 7.1 转义反引号

`` Use `code` in your Markdown file. ``

```markdown
`` Use `code` in your Markdown file. ``
```

### 7.2 代码块

    	<html>
    	  <head>
    	  </head>
    	</html>

```markdown
    	<html>
    	  <head>
    	  </head>
    	</html>
```

## 8. 分隔线语法

Try to put a blank line before...

---

...and after a horizontal rule.

```markdown
Try to put a blank line before...

---

...and after a horizontal rule.
```

## 9. 链接语法

`[超链接显示名](超链接地址 '超链接title')`
这是一个链接 [chinrunja 的博客](https://github.com/chinrunja/Blog).

```markdown
这是一个链接 [chinrunja 的博客](https://github.com/chinrunja/Blog).
```

### 9.1 给链接增加 Title

这是一个链接 [chinrunja 的博客](https://github.com/chinrunja/Blog 'somewhere for writing').

```markdown
这是一个链接 [chinrunja 的博客](https://github.com/chinrunja/Blog 'somewhere for writing').
```

### 9.2 网址和 Email 地址

<https://github.com/chinrunja/Blog>

<chinrunja@github.com>

```markdown
<https://markdown.com.cn>
<chinrunja@github.com>
```

### 9.3 带格式化的链接

I love supporting the **[EFF](https://eff.org)**.
This is the _[Markdown Guide](https://www.markdownguide.org)_.
See the section on [`code`](#code).

```markdown
I love supporting the **[EFF](https://eff.org)**.
This is the _[Markdown Guide](https://www.markdownguide.org)_.
See the section on [`code`](#code).
```

### 9.4 引用类型链接

## 10. 图片语法

![Tux, the Linux mascot](./img/linux.png 'Linux mascot')

```markdown
![Tux, the Linux mascot](./img/linux.png 'Linux mascot')
```

### 链接图片

[![Tux, the Linux mascot](./img/linux.png 'Linux mascot')](https://linux.cn)

```markdown
[![Tux, the Linux mascot](./img/linux.png 'Linux mascot')](https://linux.cn)
```

## 11. 转义字符语法

\* Without the backslash, this would be a bullet in an unordered list.

```markdown
\* Without the backslash, this would be a bullet in an unordered list.
```

# 扩展语法

## 1. 表格

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

```markdown
| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |
```

### 1.1 对齐

| Syntax    | Description |   Test Text |
| :-------- | :---------: | ----------: |
| Header    |    Title    | Here's this |
| Paragraph |    Text     |    And more |

```markdown
| Syntax    | Description |   Test Text |
| :-------- | :---------: | ----------: |
| Header    |    Title    | Here's this |
| Paragraph |    Text     |    And more |
```

## 2. 围栏代码块

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

```markdown
\`\`\`
{
"firstName": "John",
"lastName": "Smith",
"age": 25
}
\`\`\`
```

### 语法高亮

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

```markdown
\`\`\`json
{
"firstName": "John",
"lastName": "Smith",
"age": 25
}
\`\`\`
```

## 3. 脚注

Here's a simple footnote, [^1] and here's a longer one.[^bignote], test [^3].
The footnote will show at the end of the doc.
[^1]: This is the first footnote.
[^bignote]: Here's one with multiple paragraphs and code.

```markdown
Indent paragraphs to include them in the footnote.
`{ my code }`
Add as many paragraphs as you like.
```

[^3]: It's the test note.

```markdown
Here's a simple footnote, [^1] and here's a longer one.[^bignote], test [^3].
The footnote will show at the end of the doc.
[^1]: This is the first footnote.
[^bignote]: Here's one with multiple paragraphs and code.
\`\`\`markdown
Indent paragraphs to include them in the footnote.
`{ my code }`
Add as many paragraphs as you like.
\`\`\`
[^3]: It's the test note.
```

## 4. 连接到标题 ID (#headid)

[基本语法](#基本语法)
[扩展语法](#扩展语法)

```markdown
[基本语法](#基本语法)
[扩展语法](#扩展语法)
```

## 5. 删除线

~~世界是平坦的。~~ 我们现在知道世界是圆的。

```markdown
~~世界是平坦的。~~ 我们现在知道世界是圆的。
```

## 6. 任务列表语法

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

```markdown
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

## 7. 使用 Emoji 表情

### 7.1 复制和粘贴表情符号

### 7.2 使用表情符号简码

去露营了！ :tent: 很快回来。
真好笑！ :joy:

```markdown
去露营了！ :tent: 很快回来。
真好笑！ :joy:
```

## 8. 自动网址链接

http://www.example.com

```markdown
http://www.example.com
```

### 禁用自动 URL 链接

`http://www.example.com`

```markdown
`http://www.example.com`
```
