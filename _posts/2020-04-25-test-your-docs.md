---
layout: post
title: "Two reasons why you should test your docs"
author: deanna
description: "Not testing your docs? You should be"
---
I forget how I stumbled about the topic of testing documentation, but I think it had something to do with Write the Docs. I knew enough about testing code, but I didn't know there were tools out there to test documentation. After poking around with a few tools and doing some reading, I've seen the light. And I want to share that light with you.

## Testing code vs. testing documentation

When software developers test their code, they may test the application's functionality or look for any security issues in their code. When technical writers test their documentation, they may check to make sure that the links aren't broken, the style is consistent, and that there aren't grammar, spelling, or punctuation errors. Here's why:

### 1. Broken links = bad user experience

Imagine that you're reading an article about mechanical keyboards because you're thinking of buying one. The author lists several links to keyboards they recommend. You click on one of the links and....nothing. The links are broken, and you get a classic 404 page.

It's happened to me, and I'm sure it's happened to you, and it's frustrating to click on a link that doesn't work. This applies to writing documentation, too. If you include links to another company's documentation, but the links are broken, your users may be frustrated, especially if they need to read that documentation to use your product.

### 2. Inconsistent style and spelling errors = bad user experience

As someone who edits technical documentation, I cannot stress enough the importance of checking your writing for style, grammar, and punctuation. I see these things as the icing on the cake. If you don't check your documentation for these things, you're giving your users cake with no icing.

#### Style

It's important to keep your style consistent across your documentation. Multiple writers often work on the documentation and not everyone writes in the same style. One writer may write in a style that's too informal. Another writer may use long, winding sentences that never end.  If you don't keep your style and voice consistent, users will encounter a different author on every page.

The best way to keep your style consistent is to use a style guide. Ideally, your company has one for you to use; if not, you can always use a third-party style guide, like the Chicago Manual of Style.

#### Grammar, spelling, punctuation

You should always make sure your documentation is free of grammatical errors, spelling errors, and punctuation errors. Misusing *its* and *it's* happens more often than you'd think. Surface-level errors affect the readability of your documentation and can also affect users' confidence in your project.

## How do you test your documentation?

Most developers and technical writers use *linters* for testing. Linters for code look for syntax errors, [code smells](https://martinfowler.com/bliki/CodeSmell.html), typos, and other bugs. Linters for documentation look for style errors, spelling and punctuation errors, check for broken links, or make sure your documentation's [accessible](https://www.uxmatters.com/mt/archives/2016/08/accessible-documentation.php).

There are several linters out there that you can use to test your documentation. Two linters I recommend are Vale Server and write-good.

### Vale Server

You can use this popular linter from the command line, or you can use their desktop application. This linter focuses on writing style.

I personally use Vale Server because you can use third-party styles with the application, like the Microsoft Style Guide or the Google Developer Documentation Style guide. In other words, if your company uses Microsoft's Writing Style Guide, you can configure Vale to catch any errors contradictory to the Microsoft style guide.

### write-good

write-good is another popular linter that also focuses on writing style and is available for use through the command line. I've found that it focuses on passive voice, wordiness, and "weasel words" (e.g. "really", "simply").

One of the benefits of write-good is that it allows users to disable certain checks (i.e. "don't check for hyphens"), or enable certain checks (i.e. "only check for passive voice"). It's customizable to your company's writing style.

## Key takeaways

* Testing your documentation can greatly improve your users' experience
* Linters for documentation can check your writing for broken links, grammar, and style
* Style guides can help you achieve consistency across your documentation

## Links to learn more

- Vale Server's [documentation](https://errata-ai.github.io/vale-server/docs/about.html)
- write-good's [documentation](https://github.com/btford/write-good)
