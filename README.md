# Useful Hugo Shortcodes & HTML

This is a collection of shortcodes and partials that I started while [migrating my gamedev blog to Hugo](https://letsmakeagame.net/static-vs-dynamic-website/).

[![Join Discord](https://letsmakeagame.net/joinDiscord.png | width=200)](https://bit.ly/3eovU6F)

## Shortcodes Usage
Copy them to `layouts/shortcodes` folder and use them depending on the shortcode itself. Or you can also add any of this reposity subfolders as [submodules](https://github.blog/2016-02-01-working-with-submodules/).

### Table of Contents
Usage: `{{< table-of-contents >}}`

### Collapsible
This may not work for some older browser versions, [see here](https://caniuse.com/details).

Usage:
``` 
{{< collapsible summary="" >}}
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
