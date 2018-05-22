---
    date: 2018-05-22
    category: First Phase
---

##### First Week Ends
14 May 2018 - 21 May 2018

<br/><br/>
Time flies by so fast! It has been one whole week since the coding
period has begun. I have been a doing a whole lot of reading up and
understanding the code. As per our agreed upon schedule this week was
devoted to designing an architecture for the language server and
figure out all the tools that we should be using.<br/><br/>

> ##### Development Updates

So, as I said, this week was all about get to know about the stuff I should
know to work on the project efficiently. As part of it I had to come up with
a project architecture, gather all the resources necessary. Here are some of
the things we achieved this week.<br/><br/>

1. **Project Architecture**: We have the project architecture designed now
   which we believe is extensible enough to support our future plans.
   <br/><br/>

2. **Project Repo**: We now have a temporary repo to hold our project hosted
   on my github profile ([coala-langserver](https://github.com/ksdme/coala-langserver/)).
   Once it matures we will merge it upstream.<br/><br/>

3. **Resources**: I have now figured out all the tools we will be using.
   Some of them are listed in the next section.<br/><br/>

4. **More discussion about project**: We have had more discussion about the
   project on the PR page of the update to projects.coala.io. My other mentor
   [@gatesn](https://github.com/gatesn) also jumped in and gave some valuable
   review comments.<br/><br/>

> ##### Things I learnt this week

Coming up with a project architecture is not as easy as it sounds. You need
to have a clear understanding of the goals, usability and the future scope
of the project beforehand. Fortunately, my project was based on an existing
project and I had some source of inspiration from the
[python-language server](https://github.com/palantir/python-language-server).
<br/>Here are some things I learnt along the way this week:<br/><br/>

1. **A whole lot about CI**: CI is awesome! To decide upon the infrastructure
   of our project I had to read how CI systems and how to configure some
   them. Fyi, we will be using [Travis](http://travis-ci.org/) and
   [AppVeyor](https://www.appveyor.com/).<br/><br/>

2. **Plugin ecosystem design**: I was evaluating our need for a plugin based
   ecosystem for the server. Although the idea sounds like an overkill
   for this use case but I wanted to leave no stone unturned. As it turns
   out we won't be using any.
   Try [pluggy](https://pluggy.readthedocs.io/en/latest/).<br/><br/>

3. **Python concurrent module**: An awesome concurrency library that abstracts
   away all the nitty gritty details of parallel execution. (yes, parallel, I
   know it can do thread and process pools).<br/><br/>

4. **LSP**: I had to read the specification again to make my understanding of
   project scope more clear and detailed.<br/><br/>

The next week will be devoted to build a basic language server with primitive
support for at least some request types. You can follow the project at the repo
mentioned above.
