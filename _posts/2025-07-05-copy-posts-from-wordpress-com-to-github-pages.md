---
title: "copy posts from wordpress.com to github pages"
date: 2025-07-05
---

so i want to create <a href="http://ferryzhou.github.io">ferryzhou.github.io</a> with my programming only posts on <a href="http://ferryzhou.wordpress.com">ferryzhou.wordpress.com</a>

started with a git repo

first use github codespace + copilot

code is here: <a href="https://github.com/ferryzhou/wp2gh#">https://github.com/ferryzhou/wp2gh#</a>

initially the generated code try to use rest api but it does not work

then i just export my wordpress content

ask copilot to write a function to read xml instead

this is much faster and data looks good

also setup <a href="https://github.com/ferryzhou/ferryzhou.github.io">https://github.com/ferryzhou/ferryzhou.github.io</a>

ask copilot to enable create pull requests

code is good

made multiple edits

the main bug is markdownify somehow strip whitespaces of the original content and it made results ugly

fixed the bug by just remove the markdownify md processing step

the other issue is that when setup <a href="http://ferryzhou.github.io">ferryzhou.github.io</a>, i forgot to start with a template

have to copy and commit

here's results: <a href="https://ferryzhou.github.io/">https://ferryzhou.github.io/</a>

pretty god

Another good thing is that I can run the code again and again, update all articles, without worry about duplication. as the each post will always has the same file name.

lastly, each update is a pull request, so I can inspect changes first.

the whole project took about several hours.

didn't manually write too much code, mostly vibe coding.

the key is to quickly iterate, verify and find the right path.
