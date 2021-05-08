# Useful Hugo Shortcodes & HTML

This is a collection of shortcodes and partials that I started while [migrating my gamedev blog to Hugo](https://letsmakeagame.net/static-vs-dynamic-website/).

<a href="https://bit.ly/3eovU6F"><img src="https://letsmakeagame.net/joinDiscord.png" width="300"></a>

## Shortcodes Usage
You can find all the shortcodes in the [`shortcodes`](https://github.com/Stals/lmg-hugo/tree/main/shortcodes) folder. 
Copy them to `layouts/shortcodes` folder and use depending on the shortcode itself. Or you can also add any of this reposity subfolders as [submodules](https://github.blog/2016-02-01-working-with-submodules/).

### Text Highlight
Usage:
```
{{< text-highlight >}}
Your highlighted text goes here
{{< /text-highlight >}}
```
You can also use other highlight colors if you just pass "Crimson", "Cyan" or any other [color names supported by modern browsers](https://www.w3schools.com/tags/ref_colornames.asp),
or specify a full color code including transparency, like `#dc143c26`
```
{{< text-highlight color="#dc143c26">}}
Your highlighted text goes here
{{< /text-highlight >}}
```

### Collapsible
This may not work for some older browser versions, [see here](https://caniuse.com/details).

Usage:
``` 
{{< collapsible summary="Click to Expand" >}}
Here goes something you want to be mostly hidden by default, but with ability to open it.
{{< /collapsible >}}
```

Use can even add other shortcodes inside the collapsible block
```
{{< collapsible summary="Code Example" >}}
{{< highlight "C#" >}}
// your code here
{{< /highlight >}}
{{< /collapsible >}}
```

### Table of Contents
Usage: `{{< table-of-contents >}}`
