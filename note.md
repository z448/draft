###todo

- implement depencdeny download for pbcopy

[drafts url scheme](https://agiletortoise.zendesk.com/hc/en-us/articles/202771400-Drafts-URL-Schemes)


Drafts: drafts4://, x-drafts4://
 
Examples
**create** a draft with the text “Hello World”:
drafts4://x-callback-url/create?text=Hello%20World

**create** a draft with the text “Hello World”, then fire the **“Copy to Clipboard**” action:
drafts4://x-callback-url/create?text=Hello%20World&action=Copy%20to%20Clipboard
