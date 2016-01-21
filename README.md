##draft
**CLI** tool for **ios** to pipe command output into **iCloud** using iOS Drafts x-callback-url

####*update*

File is now markdown instead of txt, piping command to draft will prepend/append bash script format. First line of note when not piping command is note title, see gif bellow for details.


So far simple Perl script that will push note from terminal into iCloud using Drafts x-callback-url for iCloud. Can by changed to support other x-callback capable apps but Drafts it's meant to be sort of middleware-for-notes.

**Setup** ( might be automated in far future )
Install Drafts from AppStore, go to settings and link your iCloud account. Then make copy of action 'Save To iCloud', rename it to 'icloud' and set following:

- filename to cli
- extension to txt
- write type to append
- content to [[clipboard]]

Clone this repo into ios and use `draft` or `dft` command w/o any option. Make some notes and press Ctrl-D at the end, your note will be pushed into iCloud on Mac.

```bash
dft
title of my note
body of note
more body
lots of bodys
   <Ctrl-D>
```

Or to pipe command output into `dft.md` file in **iCloud** on Mac which can be found in `/Users/z/Library/Mobile\ Documents/iCloud~com~agiletortoise~Drafts4/Documents`

```bash
ls -la | dft
```

**gif**

![clicl](https://raw.githubusercontent.com/z448/clicl/master/clicl.gif)


