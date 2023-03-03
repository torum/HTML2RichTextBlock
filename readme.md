This is a WinUI3 (Windows App SDK) class library to display HTML in a RichTextBlock easily

**Usage:** 

1) In a XAML file, declare the namespace:

```xaml
xmlns:html="using:HTML2RichTextBlock"
```

2) In RichTextBlock controls, set or databind the Html property: 

```xaml
<RichTextBlock html:HtmlProperties.Html="{x:Bind ViewModel.Content, Mode=OneWay}" />

```

or 

```xaml
<RichTextBlock>
    <html:Properties.Html>
        <![CDATA[
            <p>This is a list:</p>
            <ul>
                <li>Item 1</li>
                <li>Item 2</li>
                <li>Item 3</li>
            </ul>
		]]>
	</html:Properties.Html>
</RichTextBlock>
```



// Code originaly adapted from https://blogs.msdn.microsoft.com/tess/2013/05/13/displaying-html-content-in-a-richtextblock/
// Modified from https://github.com/xleon/HTML2XAML/blob/master/XAMLHtml/XAMLHtml.cs