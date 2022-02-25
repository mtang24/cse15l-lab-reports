# Lab Report 4 - Week 8

View all my lab reports [here](https://mtang24.github.io/cse15l-lab-reports/)!

---

For reference, these are the `markdown-parse` repositories used:

* [Mine](https://github.com/mtang24/markdown-parse)
* [The other group's](https://github.com/BenX-64/markdown-parse)


## Snippet 1

Using the CommonMark demo site, Snippet 1's code should produce only the second line of text as a link:

[another link](`google.com)`

This means that `[google.com]` should be returned.

To test the output of this link in `markdown-parse`, I created the following test:

![Image](lr4-pics/snippet1test.png)

In my implementation, the test did not pass:

![Image](lr4-pics/mysnippet1.png)

In the implementation of another group, the test did not pass either:

![Image](lr4-pics/othersnippet1.png)


## Snippet 2

Using the CommonMark demo site, each line of Snippet 2's code should a link. However, the first line of text should only return `a.com` and not `b.com`:

[nested link](a.com)

[a nested parenthesized url](a.com(()))

[some escaped \[ brackets \]](example.com)


This means that `[a.com, a.com(()), example.com]` should be returned.

To test the output of this link in `markdown-parse`, I created the following test:

![Image](lr4-pics/snippet2test.png)

In my implementation, the test did not pass:

![Image](lr4-pics/mysnippet2.png)

In the implementation of another group, the test did not pass either:

![Image](lr4-pics/othersnippet2.png)

## Snippet 3

Using the CommonMark demo site, Snippet 3's code should produce only the third group of lines of text as a link:

[this title text is really long and takes up more than 
one line](
    https://ucsd-cse15l-w22.github.io/
)

This means that `[https://ucsd-cse15l-w22.github.io/]` should be returned.

To test the output of this link in `markdown-parse`, I created the following test:

![Image](lr4-pics/snippet3test.png)

In my implementation, the test did not pass:

![Image](lr4-pics/mysnippet3.png)

In the implementation of another group, the test did not pass either:

![Image](lr4-pics/othersnippet3.png)


## Potential Code Changes