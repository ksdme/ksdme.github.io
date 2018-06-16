---
    date: 2018-06-11
    category: First Phase
---

##### Fourth Week Ends
4 June 2018 - 11 June 2018

<br/><br/>
This marks the end of week 4, and by extension also means that now the
evaluations for phase one are open. We had a lot of meetings this week
to make sure that we are covered for the evals. I had a few minor tasks
that I totally forgot about but @gaocegege made sure I completed them.
One thing I feel obliged to write about is how I screwed up again by
pushing a huge tangled mess of code without any neat structure. Again, my
mentor was cool enough about it and dragged me through the situation and
helped me restructure the code to an acceptable form.  I think I will make
it a priority to not repeat any such behavior and keep my code changes atomic
enough.

<br/><br/>
> ##### Developments

This week included a lot of code refactoring and all the other stuff you do
to it to make it more readable and maintainable.<br/><br/>

1. <br/>**Commit Restructuring**:
   As mentioned above I had previously maintained a 'not-so-logical' commit
   history and this was once again turning into a problem for getting the
   code rapidly reviewed and merged. I fixed all of the commit history
   to at least help the situation a tad more.<br/><br/>

2. **Performance Metrics**:
   One of our tasks for Phase-1 was to have initial performance metrics for
   the coala language server. I chose to write a script that automates the
   raw metric data collection. The data although needs some processing to
   get it into an insightful form.<br/><br/>

3. **m_exit**:
   The language server was missing support for exit notification which was
   later implemented in this phase.<br/><br/>

4. **Tests**:
   The tests were using nix based file paths which could've been a problem for
   testing on Windows, hence they were improved to support an OS independent
   test suite. Some changes introduced during the code restructuring and
   supporting the missing notification required extending the tests and
   improving upon them too.<br/><br/>

5. **Docs**:
   One of the important things that I did not touch upon in the early stages
   of developement was documenting the code. This was a Phase-1 task and I
   thus added documentation to every single public entity of the project.
   <br/><br/>

<br/>I think we are covered for the Phase-1 wvals, even though I had been
behind on my schedule more than a few times we pulled off and completed all
the tasks on time. Since this could as easily be my last post from GSoC-18,
I want to highlight that this has been a great experience If not anything I
have improved vastly upon my code management skills which I now realize I was
terrible at. I have also got to know a lot of cool people because of this.
<br/><br/>

_**Update**_: I got an email from Google saying I have passed Phase-1! I look
forward to work even more tirelessly. Thanks to all for helping me get through.
