---
    date: 2018-06-28
    category: Second Phase
---

##### Code, Write.
28 June 2018 - 4 July 2018

<br/><br/>
This is a backdated post. This is going to be fun.

So, last week I had `textDocument/formatting` working so you
can now fix some/all of your code linting issues. This week
it was the time to begin development of the vscode plugin for
the coala-ls, so you, yes YOU, can use coala more efficiently
via the coala-ls I was developing. The good news is we do not
need many changes to the existing vs-code client, the one
@gaocegege developed back in the day. The worst part is vscode
plugin needs to be written in TypeScript. I have not been a big
user or proponent of node, so I never really learnt this famous
type checked flavor of JavaScript. Well, its apparent now I think,
I will have to learn at least some TS. So, here we go, this is a
brief of all the developments happened during the week.

> ##### Developments

1. <br/>**textDocument/formatting**:
   Completed the support for formatting, coala-ls now has docs,
   tests and complete support for formatting.<br/><br/>

2. **coala-vs-code cleanup**:
   Earlier the repository used to contain a language server built
   specifically for vscode, from now on it will be used to host the
   language server client. Repository wide clean up is thus required.
   <br/><br/>

3. **coala-vs-code extension**
   Improves the extension by allowing to be user/workspace configurable,
   currently supports `coalals.maxWorkers` and `coalals.tcpPort`. It also
   is invoked for all the supported languages. This filter will further
   finished during phase 3 when some cEP proposals are implemented.
   <br/><br/>

4. **Completed cEP**
   Finally, the long standing cEP is now complete and has been put up
   for review. The cEP is about optimizing coala core for being better
   compatible with language server. The current proposal is so designed
   to produce minimal changes to the coala core. It is now cEP-0028.
   <br/><br/>

To summarize, I worked with node, TS, completed my cEP and got the vscode
client working in both TCP and IO modes.
