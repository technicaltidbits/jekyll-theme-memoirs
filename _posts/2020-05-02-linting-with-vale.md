---
layout: post
title: "Linting files with Vale: an introduction"
author: deanna
comments: true
---
My journey into learning more about testing documentation began a few months ago. I joined the Write the Docs [Slack](https://www.writethedocs.org/slack/) group because I wanted to learn more about technical writing trends and tools. As I learned more about technical writing tools and processes, one term came up a few times: docs as code.

A quick Google search told me that docs as code essentially means:

* Writing your documentation with the same tools you do code
* Writing your documentation files in a markup language like Markdown or Asciidoc
* Storing your doc files in a version control system, like Git
* Building and deploying a documentation site
* Testing your documentation

I work on a team that uses the docs as code workflow to some extent, so I was familiar with writing documentation in Markdown and using Git for version control, and somewhat familiar with building and deploying a documentation site, but I had no experience with testing documentation. So I decided to learn more about it.

---

If you read my previous [post](https://technicaltidbits.net/journal/test-your-docs/), technical writers and other documentation specialists use **linters** to test their documentation.

>Linters for code look for syntax errors, code smells, typos, and other bugs. Linters for documentation look for style errors, spelling and punctuation errors, or broken links.

Two popular linters I've learned about are write-good and Vale. Both are useful for writers looking to make sure that their documentation has a consistent style, consistent tone, and no spelling/grammar errors.

If you're interested in using Vale, you can either use the desktop application, Vale Server, or the command-line interface (CLI) for linting. I personally like Vale because you can customize it to use third-party styles or even create your own rules specific to your company's brand guidelines.

Because docs as code and testing documentation are growing in popularity, I thought it'd be useful to write a three-part series that teaches the basics of using Vale. This series will focus on the CLI, not the application.

By the end of the series, you'll know how to install, configure, and lint your own documentation files. Look out for part one soon!

## Further reading

### Docs as code

* Tom Johnson's blog post about [docs as code tools](https://idratherbewriting.com/learnapidoc/pubapis_docs_as_code.html)
* Anne Gentle's book, [Docs Like Code](https://www.amazon.com/dp/B0784ZJWSR/ref=dp-kindle-redirect?_encoding=UTF8&btkr=1)

### Testing documentation

* More about testing documentation from [Write the Docs](https://www.writethedocs.org/guide/tools/testing/)

### Vale

* [Vale CLI website](https://github.com/errata-ai/vale)
