# ctags for Markdown + frontmatter + tags

```
---
title: my document with frontmatter
tags: [ hello, world ]
---
# Normal markdown from here
## But with minor changes
ctags will pick up @tags with an 'at'.
```

# What does it do?

With this configuration file [universal ctags](ctags.io) can understand the
above markdown file.
It will create a ```tags``` file that editors and programming IDEs use to index
projects and help you navigate across files.

# Installation

Place the ```vorg.ctags``` somewhere ctag can pick it up.  For instance, at the
root of your project, in a ```.ctags/``` folder.

The language name (```langdef``` for ctags) I use is ```vorg```: the name of my
vim based note keeping setup.
