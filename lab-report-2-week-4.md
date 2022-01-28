# Lab Report 2 - Week 4

## Code Change 1

![Image](change1.png)

This [test file](https://github.com/mtang24/markdown-parse/blob/main/test-file2.md) caused a failure-inducing input that prompted the changes made above.

Before making that change, running the markdown file would result in the following:

![Image](change1symptom.png)

**What happened here?**
The test file containing the failure-inducing input contained a link that was formatted incorrectly, using a `)` instead of a `]`. This created a bug in `MarkdownParse.java`, as this file was only expecting a close bracket at that index instead of a close parenthesis. As a result, running this code produced a noticeable symptom: an infinite loop printing `-1`.



## Code Change 2

![Image](change2.png)




## Code Change 3

![Image](change3.png)

