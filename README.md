# 洞见的Markdown语法

制定这个语法标准，是希望简化洞见的文字编辑流程，比如从Google Doc转换成Markdown格式。

同时用尽量少的Markdown语法标签，就可以描述不同作者的文章内容结构，达到最后洞见统一的呈现效果。

同时可以逐渐教育洞见写作者良好的写作习惯。

以下是一个范例：

--

# 这个是文章标题，使用一个#号

这里是正文的开始，段首不要缩进，顶格会让文章看起来更整齐。**粗体用这个样式**。

### 这是一级小标题，使用三个#号

然后这里是正文部分。

#### 这是二级小标题，使用四个#号

正文的段落不要太长，就这么长就可以了，及时分段，大段的文字会让读者产生疲惫感。正文的段落不要太长，就这么长就可以了，及时分段，大段的文字会让读者产生疲惫感。正文的段落不要太长，就这么长就可以了，及时分段，大段的文字会让读者产生疲惫感。正文的段落不要太长，就这么长就可以了，及时分段，大段的文字会让读者产生疲惫感。正文的段落不要太长，就这么长就可以了，及时分段，大段的文字会让读者产生疲惫感。

--

有序号的列表格式：

1. 有序号的列表
2. 有序号的列表
3. 有序号的列表 

无序号的列表格式：

* 无序号的列表
* 无序号的列表
* 无序号的列表


一般不推荐嵌套列表，如果非要用，有序和无序号需要错开使用：

1. 有序号的列表
	* 无序号的列表
	* 无序号的列表
		1. 有序号列表
		2. 有序号列表
2. 有序号的列表
	* 无序号的列表
		1. 有序号列表

-- 

下面是引用的示例：

> 比如这是我说的一段话。比如这是我说的一段话。比如这是我说的一段话。比如这是我说的一段话。比如这是我说的一段话。比如这是我说的一段话。比如这是我说的一段话。

--

下面是链接的示例：

[ThoughtWorks的敏捷开发](https://insights.thoughtworks.cn/agile-development-thoughtworks/)

--

下面是图片示例：

![这是图片的alt信息，一定要加上。注意图片的文件名需要是有意义的命名](https://insights.thoughtworks.cn/wp-content/uploads/2020/04/1-remote-cooperation.jpg)

-- 

文字中代码示例，比如这个单词`builtIns`就是代码。

--

下面是多行代码示例：

```
const builtIns = {
    minLength: (value, criteria) => value && value.length > criteria,
    maxLength: (value, criteria) => value && value.length < criteria
}

const isValid = (validations) => (value) => {
    return _.every(validations, (k, v) => builtIns[k](value, v))
}

const AddressSearch = ({validations, value}) => (<Input error={isValid(validations)(value)} ... />);
```

--
下面是表格的示例：

|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |
--

##### 这是三级小标题，使用五个#号。但一般不推荐用，建议作者也不要用。或者编辑自行修改掉。

--

### 这是第二个小标题，使用三级标题标签

--

****

### 小结的小标题，一般文章的都会有一个，也使用三级标题标签

--

参考Markdown编辑器
* MacDown
* MarkEditor（Markdown）
* Ulysses
* Bear
