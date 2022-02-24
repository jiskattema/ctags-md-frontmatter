# ctags for Markdown + frontmatter + tags

```
---
title: my document with frontmatter
tags: [ hello, world ]
---
# Normal markdown from here
## But with minor @changes
ctags will pick up @tags with an 'at'.
```

# What does it do?

With this configuration file [universal ctags](ctags.io) can understand the
above markdown file.
It will create a ```tags``` file that editors and programming IDEs use to index
projects and help you navigate across files.

From the example above, we will get the following tags:

 * ```@hello``` and ```@world``` from the frontmatter line starting with ```tags:```. The tag type is ```D```.
 * ```# Normal markdown from here``` a heading by the regular Markdown parser
 * ```## But with Minor @changes``` a heading by the regular Markdown parser
 * ```@changes``` and ```@tags``` tags in the Markdown, because it starts with ```@```, type ```f```

# Installation

Place the ```vorg.ctags``` somewhere ctags can pick it up.  For instance, at the
root of your project, in a ```.ctags/``` folder.

The language name (```langdef``` for ctags) I use is ```vorg```: the name of my
vim based note keeping setup.

ctags applies this ```langdef``` for suffixes ```txt``` and ```md```.
