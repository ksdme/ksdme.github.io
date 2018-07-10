---
    date: 2018-07-05
    category: Second Phase
---

##### The End of Times.
04 July 2018 - 10 July 2018

<br/><br/>
So, the end of Phase-2 of GSoC 18 is about to begin in
a few hours, It feels like the second phase passed
blazing fast. This period got more packed than I could
have imagined mostly due to some personal things that
required my attention. I feel it quite important to mention
that my mentor @gaocegege was quite positive about it and
helped me in every manner possible even when his schedule
got a bit too packed. @gaocegege Thanks!.

Second phase was mostly about supporting `formatting` and
producing a vscode client for coalals. I think we achieved
those goals to an acceptable level, although we have our
PR's pending for review, the architecture was discussed
beforehand so no major issues must've propagated through.
Currently, the newer version of coala-vs-code is installable
from the vscode marketplace you will be required to install
coalals manually and merge the code on you local dev env to
test it out. This should flawlessly work when coalals is
made available via PyPi.

> ##### Developments

Here are the developments from the last week of development
specifically.

1. <br/>**Support window/showMessageRequest**:
   `window/showMessageRequest` can be used to alert the end user
   about some event or an option and the feedback can be collected
   and processed. The support comes to the LangServer class but is
   currently not used in any place as is. This could be useful for
   future developments such as in event of Phase-3.<br/><br/>

2. **Tests**
   coala-ls yet again has complete coverage of tests. It now features
   almost 80+ tests.<br/><br/>

3. **Docs**
   coala-ls also features complete docs.<br/><br/>

4. **Performance Metrics**
   We have the performance metrics in place for the additional features
   introduced in this phase i.e `textDocument/formatting`.<br/><br/>

5. **coala-vs-code tests**
   Because of the pending PR status of coalals, End to End tests are
   tough to design because of the local merges required. Hence, basic
   unit tests are available for coala-vs-code.<br/><br/>

6. **Demonstration Video**
   As described in the requirements, we have a video demonstrating the
   capabilities of the coala-ls and coala-vs-code.<br/><br/>

> ##### Links

1. **coala-ls**: http://github.com/coala/coala-ls/pulls/<br/>
2. **coala-vs-code**: https://github.com/coala/coala-vs-code/pulls<br/>
3. **Videos**: https://www.youtube.com/watch?v=MeybdlCB96U &
   https://www.youtube.com/watch?v=uOnFQqe0IjU<br/>

Huh, we are here, this marks the end of the blog post. Wish we luck for
the evals.
