---
    date: 2018-06-27
    category: Second Phase
---

##### Second Phase, Yay!.
12 July 2018 - 27 July 2018

<br/><br/>
So, I passed the first phase. I would like to take a moment to thank
my mentors especially @gaocegege and the org admin @jayvdb. All the
mentors and fellow students who helped me build my language server,
thank you! I am gald that I have passed phase one. It is now time to
improve the language server to support yet some more request types on
the server and polish the VS Code plugin.

This blog post accounts for the past two weeks. Now that I am finally
done with my exams and the vacations have started I travelled back to
my home and started working on the tasks for Phase 2. As mentioned
above Phase 2 involves improving the server and working on the client.

I picked working on expanding the server request type support
to begin with. Our prime goal was to support `textDoument/formatting`
and a few others. `formatting` is intended to fix the issues related
to spacing and indentation in the code but initially coala ls will
fixing all the code irrespective of the type of the patch. This can
get tricky at times when the diffs are overlapping. I am confident
that some additional changes introduced during Phase 3 will solve
those issues and make formatting a feature to be used regularly.

> ##### Developments

The past two weeks mainly involved researching about the `formatting`
and completing some back logs. Anyway, here are a few developments.

1. <br/>**Refactoring**:
   The `coalals.results` module was refactored to make it make into
   a sub module, now with `coalals.results.diagnostics`.<br/><br/>

2. **Support code fixes**:
   Added `coalals.results.fixes`, now the diffs generated by the
   coala core can be parsed into coalaPatch objects.<br/><br/>

3. **Misc Changes**:
   Some additional changes have been introduced wherever required to
   support the new `formatting` request type.<br/><br/>

4. **Supports `textDocument/formatting`**:
   coala language server now supports `formatting` requests. Initially
   this does not fix all the issues but skips any overlapping changes.
   Here is a sneak peak: ()[https://youtu.be/uOnFQqe0IjU]<br/><br/>

5. **Adds Tests**:
   The coverage of the tests has been bumped to 100%. All the newly
   added code is covered by the tests too.<br/><br/>

6. **Docs**:
   As usual, all the code has been properly documented.<br/><br/>

We now have a working implementation of code fixing in the editor itself
using coala and the `formatting` requests. My mentor and I have decided
on how to implement and work with the VS Code plugin.