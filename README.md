# clicl
**CLI** tool for **ios** to pipe command output into **iCloud** using x-callback-url

So far simple Perl script that will push note from terminal into iCloud using Drafts x-callback-url for iCloud. Can by changed to support other x-callback capable apps but im using Drafts ever since i lost JB, and it's meant to be sort of 'middleware-for-notes'.

**Setup** ( might be automated in far future )
Install Drafts from AppStore, go to settings and link your iCloud account. Then make copy of action 'Save To iCloud', rename it to 'icloud' and set following:

- filename to cli
- extension to txt
- write type to append
- content to [[clipboard]]

Clone this repo into ios and use `clicl` or `icl` command w/o any option. Make some notes and press Ctrl-D at the end, your note will be pushed into iCloud on Mac.

```bash
icl
title of my note
body of note
more body
lots of bodys
   <Ctrl-D>
```

Or to pipe command output into icli.txt file in iCloud on Mac which can be found in /Users/z/Library/Mobile\ Documents/iCloud~com~agiletortoise~Drafts4/Documents

```bash
ls -la | icl
```

**gif**
![control](https://raw.githubusercontent.com/z448/clicl/clicl.gif)

