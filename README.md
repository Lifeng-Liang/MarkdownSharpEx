MarkdownSharp
==========

���
----------

[MarkdownSharp](https://code.google.com/p/markdownsharp/) �� [Stack Overflow](http://stackoverflow.com/) ��Դ������ Markdown �� C# ʵ�֡�

����Ҫ�޸������¼��㣺

1.	���� CodeClass ���ã����ں� [prettify](https://code.google.com/p/google-code-prettify/) ��ϣ����﷨������
2.	���Ӷ��� \`\`\` ���ִ���綨������֧�֣����ں� Github ����ͬһ�� Markdown �ļ���
3.	����ǿ������ʹ֮��������Ҫ��ǿ�����ĳ��ϡ�

�޸Ļ��� markdownsharp-20100703-v113 ���С�

ʹ��
----------

���е� CodeClass����һ�����ã������� prettify������������ķ����������ã���ʹ�á�

```c#
public static string MarkdownEncode(this string s)
{
	var md = new MarkdownSharp.Markdown();
	md.CodeClass = " class=\"prettyprint\"";
	return md.Transform(s);
}
```
