---
    date: 2018-05-29
    category: First Phase
---

##### Two Weeks Flyby
21 May 2018 - 4 June 2018

<br/><br/>
A busy two weeks. I had quite a few exams in the first week and the
coding period was to begin in the very same week. And because of that I
could not put in all the time I wish I had. My mentor was understanding
of the fact and told me he was fine with it if I could get back on track
by putting more time in the subsequent days. So, I did. Once the first
week ended I had a lot time for the next exam.

I have three major tasks for this phase, to design the architecture of ls,
build a minimal language server and have complete test coverage and docs for
it. Because of support from one of my mentors (@gatesn) and the arch we
decided upon, the second task's goals were either almost readily done or
were an intersecting part of the first task. So, I did complete writing a
minimal functional server by the time of writing this blog along with tests.
The codebase is a major rewrite, so I am awaiting review for it as of now.
And, as it turns out the jekyll blog template I was using wasn't as per the
guidelines of the org and thus I had to port the entire blog to medium. I
intend to keep this version alive until the end of GSoC, but you can follow
the medium blog at [@ksdme, coala and gsoc](https://medium.com/ksdme-coala-and-gsoc).

> ##### Development Updates

This was an active week and I had many changes done to the code base as a
part of it. The PR's are awaiting review. Here are the few development
updates.<br/><br/>

Checkout the PR and codebase at:<br/><br/>

1. [https://github.com/coala/coala-ls/pull/2](https://github.com/coala/coala-ls/pull/2)<br/>
2. [https://github.com/ksdme/coala-ls/tree/gsoc-phase-1-tests](https://github.com/ksdme/coala-ls/tree/gsoc-phase-1-tests)

3. <br/>**Project Refactor**: The very first thing I did to the codebase was to
   refactor it heavily. The current implementation was not designed to be
   extensible. This was fixed by improving the code structure making it
   more modular and removing any code specific to vs-code.<br/><br/>

4. **Added Concurrency**: The server now handles the coala analysis requests
   concurrently. This now makes it possible to work on multiple files at once
   and not miss any updates during the analysis cycles. The concurrency
   infrastructure has been heavily abstracted to keep the scheduling of
   those jobs intelligent enough and keep the future updates to the interface
   module in phase 3 in mind.<br/><br/>

5. **Added FileProxy**: During certain notifications such as didChange the
   changes made to the source files are not yet flushed to the disk and using
   current coala interface configuration it is not possible to analyse those
   changes. FileProxies provide a mechanism to support such situations by
   directly providing access to the file contents and some meta information.
   FileProxies have been implemented and integrated into the module but it'll
   have to wait until the coala inteface improves in Phase 3 before making
   full use of them.<br/><br/>

6. **Partial support for didChange, didClose**: The goal for first phase
   was to extend support for didOpen and didSave. They are currently supported
   and I have even extended partial support to didChange (updating
   corresponding proxies) and handling proxies on closing a file using
   didClose notification.<br/><br/>

7. **Tests**: Previously, the tests were fragmented as behave tests and
   unittests. I have rewritten some of those tests and extended them to
   the code that was now introduced. The test suite is now unified and is
   written in pytest.<br/><br/>

Although I am glad that I have pulled off major goals of the Phase 1, some
other important goals are in back logs. I intened to complete most of them
in the days remaining before the end of Phase 1. Some of them are:<br/><br/>

1. **Docs**: The codebase only has some comments thrown around sparingly.
   I intend to write the docs for the entire code base.<br/><br/>

2. **Configure CI**: The CI needs to be configured to run the tests etc.
   I am awaiting for the initial PR to be merged to get working on the
   second issue.<br/><br/>

3. **Design Doc**: The official design doc for the architecture is still in
   WIP and needs to be submitted asap. This has the highest priority in my
   list as of now.<br/><br/>

So, overall I am glad that the server works satisfactorily. I still can't be
sure of it until it passes the review though. But, I am hoping for the best.
See you next week!.
