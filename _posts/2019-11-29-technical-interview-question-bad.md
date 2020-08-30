---
layout: posts
title: "The Dreaded Technical Interview Question"
---
*Author: Bianca Yang*<br>
*Email: <a href="mailto:ipacifics@gmail.com?subject=Hello from the XDRT Blog">ipacifics@gmail.com</a>*<br>

Update (8/29/2020): The ability for a candidate to complete a take home
assignment presumes that they have the
[privilege](https://belkadan.com/blog/2016/05/So-You-Want-To-Be-A-Compiler-Wizard/#on-free-time)
of time to complete such a task. I don't have a well codified set of principles
for running good real-time technical evaluations, so let me just paste a bunch
of thoughts and stories and come back to the harder problem of distilling them
later.
* Optimize the problem for expansion and back and forth discussion between the
interviewer and candidate on actual design considerations of space and speed.
* Let the candidate guide the discussion and implementation. Your
role as an evaluator is to push back on design choices or add complexity and
constraints to the problem definition.
* (??) Treat the candidate as though they were already a coworker.
* Try to offer a problem or environment that most closely replicates their
future day responsibilities.

Here's a couple of stories about good technical interviews I've had:
I had a great experience at Evernote where the interviewer offered me the choice
of working on a traditional algorithms / data structures problem or debugging
and patching a piece of sample code. I chose the latter problem (figured it
would be easier and more representative of day to day work). It was fun and far
less stressful than an algorithms question. I impressed the interviewer but
didn't end up moving forward in the process.

I had another good experience working on a simulated work environment problem
during an onsite interview with [Elementary Robotics](https://www.elementaryrobotics.com).
The team built a simulator environment with a robotic arm with a camera on the
end effector. They asked me to program the robot to pick up some colored blocks
and put those blocks into a holding container. In another round of the onsite
with Elementary, I wrote a hash map from scratch with the CTO. It was more
stressful in the moment than it should have been; we were working together
almost like a tutor and a student, rather than as test examiner and examinee.

I had another interesting experience with [Grail](https://grail.com) where the
interviewer had me code up a program to return the top 10 items in a list of
two field jsons by some numerical field. Once I finished the basic
implementation, he asked me some follow up questions about trading off space and
time complexity. We had time left over, so he then asked me a question that
could have gone to the [ends of the earth](https://danluu.com/navigate-url/).
The question was about debugging a shared online coding interface like coderpad.
His plan was to say "no that wouldn't work" to every suggestion for debugging I
had and see how far my knowledge of some networked computer architecture could
go. Definitely a fun problem but I was kind of exhausted by this point in the
interview and was grateful he only put me through a few rounds of "no's".

Update (8/5/2020): Building up on the 7/22/2020 update, this take home problem
should be publicly available and clearly accessible from the company's careers
page. [Iris
Automation](https://drive.google.com/drive/folders/0B50bwdqRospTRU1PejNyMldLNnc)
is the only company I know that's done this. They're a drone company that's
working on BVLOS (beyond visual line of sight of the human pilot) drone
technology. The task they designed was to develop a computer vision algorithm
that could provide as much human relevant contextual awareness as possible about
a static image. Anybody could take the challenge; anybody could submit their
solution to the email provided in the README. It should not take very long for
a company's engineers to draft up such a task and an associated rubric. It is an
effective filtering function for a candidate's raw technical ability and
provides great fodder for deeper technical discussions with the company's
employees. It also avoids the insidious problem of relying on completion of
common pathways to a certain end of experience (ahem 4 year or higher CS degree
at a reputable university) to evaluate a candidate's worthiness.

Update (7/22/2020): I now think that companies should design take home problems
that take around 4 hours to complete and that comprehensively covers what they
expect candidates to do in their day to day work. An evaluation rubric must also
be created for this assessment to reduce individual evaluator bias. Because this
test is comprehensive, any candidates who successfully meet the marks on the
rubric should be invited to meet with key team members on site (or whatever your
version of a final interview round is) for a series of discussions. The
candidate has already demonstrated sufficient technical capability, so these
discussions should be more casual and be focused on evaluating culture fit,
alignment with company vision, expected tenure, and potential growth vectors or
breadth of knowledge. [Emerald Cloud Lab](https://www.emeraldcloudlab.com) did
this with me. I spent the onsite eating meals with the team chatting about my
philosophical alignment on Thielian principles with the head of culture, and
generally getting a feel for the people who made up the design / eng / science
teams.

Update (12/7/19): For phone interviews, I now use
[Steve Yegge's Five Essential Phone Screen Questions](https://sites.google.com/site/steveyegge2/five-essential-phone-screen-questions). I haven't decided
what is best to ask for on sites...

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
