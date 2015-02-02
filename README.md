MarkdownSharp
==========

简介
----------

[MarkdownSharp](https://code.google.com/p/markdownsharp/) 是 [Stack Overflow](http://stackoverflow.com/) 开源出来的 Markdown 的 C# 实现。

我主要修改了以下几点：

1.	增加 CodeClass 配置，用于和 [prettify](https://code.google.com/p/google-code-prettify/) 配合，做语法高亮。
2.	增加对于 \`\`\` 这种代码界定方法的支持，便于和 Github 共用同一个 Markdown 文件。
3.	增加强命名，使之可以用于要求强命名的场合。

修改基于 markdownsharp-20100703-v113 进行。

使用
----------

其中的 CodeClass，是一个配置，如果配合 prettify，可以用下面的方法进行设置，并使用。

```c#
public static string MarkdownEncode(this string s)
{
	var md = new MarkdownSharp.Markdown();
	md.CodeClass = " class=\"prettyprint\"";
	return md.Transform(s);
}
```
