---
layout: post
title: "Configuring the Vale CLI"
comments: true
author: deanna
image: assets/images/vale-demo.png
---

As I mentioned in the first part of the series, in the second part, you'll learn how to configure the Vale CLI for your documentation needs. Before you dive into the tutorial, you need to learn a thing or two about the file that makes linting with Vale possible: the `.vale.ini` file.

## What is the .vale.ini file?

The `.vale.ini` file is a configuration file that tells Vale what files to **lint**, or check, what styles to conform to, and what rules to ignore. Essentially, it controls everything Vale does for you.

> Q: *Why is there a period in front of the filename?*
>
> A: Any filename that begins with a period is called a **hidden file**. Hidden files are usually tucked away for a good reason: they're files that you probably shouldn't touch unless you know what you're doing.

> Q: *What does `.ini` mean?*
>
> A: The `.ini` extension indicates that this is an [**initialization**](https://www.lifewire.com/how-to-open-edit-ini-files-2622755) file.

## .vale.ini features

Here's a basic, bare-bones `.vale.ini` file:

```ini
StylesPath = styles

MinAlertLevel = suggestion

[*] the asterisk means "apply these styles to all files" and is required.
BasedOnStyles = Vale
```

It has several *properties*: `StylesPath`, `MinAlertLevel`, and `BasedOnStyles`.

### StylesPath
`StylesPath` tells Vale where to look for third-party styles. In this example, all third-party styles are in the `styles` folder.

### MinAlertLevel

When you run the Vale CLI, it displays the number of errors, warnings, and suggestions found in the file. Errors are highest in severity; suggestions are lowest:

```ini
2 errors, 3 warnings and 3 suggestions in 1 file.
```

If you want, you can configure Vale to show errors only, errors and warnings, or show errors, warnings, and suggestions. For example, if you set `MinAlertLevel` to `error`, it only shows errors found in the file:

```ini
2 errors, 0 warnings and 0 suggestions in 1 file.
```

If you set `MinAlertLevel` to `warning`, it only shows errors and warnings:

```ini
2 errors, 3 warnings and 0 suggestions in 1 file.
```

If you set `MinAlertLevel` to `suggestions`, it shows errors, warnings, and suggestions:

```ini
2 errors, 0 warnings and 3 suggestions in 1 file.
```

### BasedOnStyles

This is the fun part.

One of the great things about Vale is that it allows you to use third-party styles with it. For example, if your company follows Microsoft's style guide, you can download a zip file containing an implementation of the Microsoft Writing Style Guide that you can use with Vale.

If you don't use a third-party style guide, you can always use the default style, which is `Vale`.

If you want Vale to implement more than one style, separate them with a comma, as shown below:

```ini
BasedOnStyles = Vale, Microsoft
```

Now, Vale uses its default style and Microsoft's style rules when linting your files.

## Key takeaways

* `StylesPath` tells Vale where to look for third-party styles.
* You can configure Vale to show errors, errors and warnings, or errors, warnings, and suggestions.
* You can use Vale's default style to lint your files, or you can use a third-party style.
* At minimum, your `.vale.ini` file must include `StylesPath`, `MinAlertLevel`, and `BasedOnStyles`.

## Conclusion

Now you know what a `.vale.ini` file is and its basic components. Next, you'll create a `.vale.ini` file and run the CLI to lint a sample Markdown file, using Vale's and Microsoft's style rules.

