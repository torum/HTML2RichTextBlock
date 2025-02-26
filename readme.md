# HTML2RichTextBlock

This is a WinUI3 (Windows App SDK) class library to display HTML fragments in a RichTextBlock.

## Usage: 

1) In a XAML file, declare the namespace:

```xaml
xmlns:html="using:HTML2RichTextBlock"
```

2) In RichTextBlock controls, set or databind the Html property: 

```xaml
<RichTextBlock html:HtmlProperties.Html="{x:Bind ViewModel.HTMLContent, Mode=OneWay}" />

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

## Limitations:
Obviously a lot. Nortably, 

* An iframe will be shown as a inline link. 
* No base url support (yet). 
* ..etc.

## Screenshot:  
![Screenshot](https://github.com/torum/HTML2RichTextBlock/blob/master/SampleScreenshotAcrylicBackdrop.png?raw=true)  

## Requirements:
* [.NET 6](https://github.com/dotnet/runtime)  
* [WinUI3 (WindowsAppSDK)](https://github.com/microsoft/WindowsAppSDK) 
* [Html Agility Pack](https://github.com/zzzprojects/html-agility-pack)

## Credits:  
- Code originaly adapted from [https://blogs.msdn.microsoft.com/tess/2013/05/13/displaying-html-content-in-a-richtextblock/](https://blogs.msdn.microsoft.com/tess/2013/05/13/displaying-html-content-in-a-richtextblock/)  

- Forked and modified from [https://github.com/xleon/HTML2XAML/blob/master/XAMLHtml/XAMLHtml.cs](https://github.com/xleon/HTML2XAML/blob/master/XAMLHtml/XAMLHtml.cs)  

 
