---
    date: 2018-07-14
    category: Third Phase
---

##### IT'S PHASE III
13 July 2018 - 30 July 2018

So, Yes, I did pass the Phase-II. This is when I should thank
my mentor (@gaacegege) and the community. Thank You!. The last phase
was all about getting the client up and running and publishing it to
the VSCode Marketplace. We did it. Now, VSCode can fix all your issues
right from your editor window and you can almost one click install
the client from the store. This phase is all about optimizing coala
and coala-vs-code. I now have a almost agreed upon cEP! Anyway here
are some developments from the past two weeks.<br/><br/>

- cEP<br/>
  coala uses something called cEP as a proposal mechanism to propose
  changes to the coala core. This is so the community can know about and
  vote on major changes. Typically cEPs are required during feature
  updates and architectural changes. Optimizing coala for coala-ls
  requires at least one feature extension and one architectural change.
  I intend to introduce a feature known as tagging, so you can conditionally
  execute a collection of sections based on the invoking tags. The
  aforementioned change to the architecture has to do with supporting
  coala execution on in-memory versions of a file rather than their
  disk counterparts.<br/>

  This cEP has been stuck in review for a month now, I have requested
  for initial approval so I can start working on the implementation,
  thanks to @shreyans800755 I have approval on implementation model of
  the tagging feature upgrade and thanks to @jayvdb I have initial approval
  on the cEP and can now start working on the implementation. Follow the cEP
  developments [here](https://github.com/coala/cEPs/pull/171)<br/>

- Prototypes<br/>
  Improving the cEP involved writing at least prototype implementations
  of the proposed changes. I have thus implemented a prototype of the proposed
  tagging feature and it functions well enough, prototype implementation of
  FileProxy support was also found to be functional enough.

- PyDelhi and coala
  Although not strictly related to this blog, I did represent coala at
  this months meetup of PyDelhi, I helped some newcomers get onboard, some
  Atleast ~10 newcomer PR's were submitted and some even got merged.

In all, the past two weeks have been mostly about working on the cEP and
getting it into an acceptable shape so I can start implementing the
proposal.
