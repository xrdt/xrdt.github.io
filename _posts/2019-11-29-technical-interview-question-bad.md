---
layout: posts
title: "The Dreaded Technical Interview Question"
---
*Author: Bianca Yang*<br>
*Email: <a href="mailto:ipacifics@gmail.com?subject=Hello from the XDRT Blog">ipacifics@gmail.com</a>*<br>

I conducted my first onsite technical interview on Thursday this past week
(11/21).
I spent a long (probably too long) time sweating over what question to ask and
even compiled a [list of questions](../../../interview.txt) I would feel
comfortable asking. Some of these questions come from my past experience.
Some of these questions come from this [Quora thread](https://www.quora.com/What-are-the-best-programming-interview-questions-youve-ever-asked-or-been-asked?share=1).
I thought about setting up a test script on my computer so candidates could
implement and test their solutions to the Leetcode style questions on my
computer but ended up not having enough motivation to do that...Yes, I'm a
lazy buttface. I'm not sure it really makes a big difference, coding on a
board vs. coding on a computer, especially since people are so primed for
it nowadays, but it certainly can make testing easier. The ease of testing
on a computer does come at some loss in analyzing a candidate's ability to
reason about a program at the most abstract level. Some candidates may rely
on the tests to determine their solution's correctness, rather than doing a
rigorous comb through just of the code. Since I would like to assess
analytical ability more than ability to debug with a computer, it probably
makes sense to continue using whiteboard coding, especially since the
questions we ask tend to not be particularly drawn out coding-wise.

I decided to ask my first candidate a medium puzzle: given an integer N,
return the number of numbers from 1 to N that have 7 as a digit. I've been
asked this question before, at a very [cool company](http://matician.com) I
did not get an offer to join. I took a *lot* of hints, but I came up with a
very compact and clean solution within 30 min max. I thought this question
would be a good way to assess the candidate's problem solving skills. But,
after running through this question twice and seeing both candidates struggle
to get the insight that would lead them to the final solution, I've given in
to my feelings that whether or not a candidate sees the nature of the problem
is somewhat random. That flash of insight we need to solve brain teasers
or riddles (??what can you take through the green glass door??) can come at
totally random times. Does measuring how long it takes someone to get to
that conclusion give a strong signal that they're worth hiring? It gives some
insight into how broad their mind is and how likely they are to get stuck on
local maxima. But I'm not sure it's effective in determining the quality of a
candidate for an entry level software engineering job (let alone any-level
software engineering job).

So, after some more nonsense self-reflection and bloating of my
[interview Q's list](../../../interview.html), I came across this awesome post
by Steve Yegge on how to do a [proper phone interview](https://sites.google.com/site/steveyegge2/five-essential-phone-screen-questions).
Steve goes over how to effectively test whether a candidate has mastered part
of the ABCs for software engineers (as he says, his list probably only goes up
to J or K). I think that any other format of interviewing (behavioral, merge
k sorted lists, design an elevator system, how many golf balls can fit in a
737, if you've traveled .5 mi @ 30mph how fast must you travel the remaining
.5 mi to make your 1mi time 1 min, etc) is totally meaningless for SCREENING
*SOFTWARE ENGINEERS*.

Onsite interviews should cover a set of topics that is a superset of what is
covered on the phone interview (perhaps letters K - Z). If the candidate
showed weakness on any of the areas during the phone, part of an onsite
interview should probe them in that area. Otherwise, onsite interviews should
be focused on forcing the candidate to prove their understanding of whatever
their resume claims they know by quizzing them about it or forcing them to
implement a related system in person. Interviewers must have clear guidelines
for what counts as acceptable performance on a question. Ideally, a script
that covers what kinds of paths candidates may take and what hints can be
given or probing questions can be asked should be given to interviewers so
the evaluation criteria are consistent. Just because you have top-notch
engineers conducting interviews doesn't mean you have a top-notch team for
filtering for quality talent. Interviewers should be coached to *drive* the
interview. Remember that you are digging for cracks, for red flags, for any
signs that the candidate would *not* be a good fit. If you ask only questions
about things the candidate has supposedly prepared a beautiful campfire
story about (ahem things on the resume) you will come away feeling impressed.
If you let the candidate wax poetic about some school project where they
implemented 5 lines of some simple web interface you will come away impressed.
You *must* know what you are looking for and demand that the candidate give
it to you. If they cannot (e.g. explain multithreading to me, complexity
analysis of the algorithm they wrote, stack vs heap), then you have found a
hole that you must mark on your rubric.

Update: Of course Steve Yegge is still the foremost authority on the topic of
how to properly conduct interviews. He published a [Medium article](https://medium.com/@steve.yegge/get-that-job-at-grab-eea6de1d8421)
in 2018 on some small updates to his approach to interviewing. The most
relevant sentence in that article about is about whether to do a breadth-first
or depth-first search into the candidate's abilities and knowledge. The
answer? Ding ding! _Breadth first_! The depth first approach of let me ask you
some modified Leetcode questions gives you such little signal. It illuminates
only the tiniest portion of the candidate's ability, leaving you still
wondering at the end of the session or even the end of four of five of these
sessions (on site interview) whether the candidate is a good engineer. That is
why I am so enamored with Yegge's five essential questions for phone screens.
Only by digging all around and poking harder at the parts that seem weird do
you get a good holistic sense for whether a candidate knows enough about
software to be useful. Anyway, I hope you read all of [Yegge's](https://steve-yegge.blogspot.com/2008/03/get-that-job-at-google.html)
posts on [interviewing](https://steve-yegge.blogspot.com/2006/03/truth-about-interviewing.html), not just the select few I've laid out here for your
perusal.

Sometimes people make a big deal out of cultural fit. Nobody wants to work
with an asshole, but unless you're running an exclusive cult I think most
people can fit into their team...What *is* an area of concern is
communication. Can the candidate explain technical concepts clearly? Do they
work well with other people? Do they know when to ask for help? Are they
receptive to feedback? Do you speak with confidence when they're right and
you're asking if they see any issues in their code?

I think that's pretty much the gamut of what matters when hiring software
engineers: technical ability and communication ability. Different things as
you go up the ladder, but I don't have good thoughts on how you judge the
capacity of a senior engineer or higher so we'll have to come back to that.

Email me to let me know if I'm wrong or missing anything. The thought of
candidates suffering through bad interview experiences keeps me up at night. I
want to make the experience a clear win-win for both the company and the
candidate and would love to know how you or your company has cracked some of
the hiring code.
