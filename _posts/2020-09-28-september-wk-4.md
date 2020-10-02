---
layout: posts
title: "September, Final Week -- OverFlow Reading"
---
*Author: Bianca Yang*<br>
*Email: <a href="mailto:ipacifics@gmail.com?subject=Hello from the XDRT Blog">ipacifics@gmail.com</a>*<br>

I was wondering why the September Wk 3 log was becoming so long...Turns out I'd
been writing in it through September 25, so I had 4 days of overflow into that
file. Oh, well...I'll continue here for the rest of the month.

__Books__:
* [二月--柔石](http://www.haodoo.net/?M=book&P=535)

__Wrackspurts__:
* You maintain largely the same personality as you get older. It's just your
  body and mental fitness that decline.

__Vicarious Conversations__:
* [DHH and Tim Ferris](https://tim.blog/2018/06/05/the-tim-ferriss-show-transcripts-david-dhh-heinemeier-hansson/)
  * Tranquility. Your expectations dominate how you feel about an outcome.
  > The best things in life are free and the next best things are very
  > expensive.
  * [It's Always Your Fault](https://m.signalvnoise.com/its-always-your-fault/)
  * Keep pulling on the thread. If it's not interesting, you haven't pulled
  enough.
  * John McPhee is a masterful writer.
* [Still Day 1](https://www.sec.gov/Archives/edgar/data/1018724/000119312517120198/d373368dex991.htm)
  * 2016 Annual Letter on Day 1 defenses:
    * Customer Obsession
    * Avoid Proxies (e.g. processes)
    * Embrace External Trends (e.g. ML)
    * Fast Decision Making

__Better Programming Tools__:
* [Bret Victor](http://worrydream.com/#!/LearnableProgramming) is the main
  contemporary guy who's working on this stuff. He of course pays homage
  to the OG researchers who figured out how to make environments that were
  actually interpretable and observable. I feel like I should paste this
  article every reading log until I'm sick of it.
  > Programming has to work like this. Programmers must be able to read the
  > vocabulary, follow the flow, and see the state. Programmers have to create
  > by reacting and create by abstracting.<br>---<br> The programming language
  > must provide identity and metaphor, decomposition,
  recomposition, and readability.
* [More Eve Stuff](https://news.ycombinator.com/item?id=12817468)
  * [The Entire Eve Bibliography](https://github.com/witheve/eve-experiments/blob/master/design/bibliography.md)
  * Can you make the environment smart enough to
   [constrain](https://news.ycombinator.com/item?id=12819742) the state space
    a programmer needs to interface with?
  * What do you do [when code and comments get out of whack](https://news.ycombinator.com/item?id=12819349)?
  How can you get better visibility into the code?
    * Code reviews exist for a reason. Enforce the discipline.
      * [Context matters](https://news.ycombinator.com/item?id=12818942)
    * Treating code as a [design
   doc](https://news.ycombinator.com/item?id=12818653). [Misalignment
      between code and comment / function name is a signal to look
   deeper](https://news.ycombinator.com/item?id=12819608). There's no way to
      enforce alignment between code and comment.
  * [A Little Context on What Eve is](http://witheve.com/deepdives/whateveis.html)
  * [Eve Comment on Prose + Code](https://news.ycombinator.com/item?id=12818076)
  * [Vim, Text++, Richer Programming
   Environments](https://news.ycombinator.com/item?id=12821039) like what CAD,
   Unity3D HyperCard, Smalltalk, etc. provide. How do you help the programmer
   interface with the semantic parts of programming (data), not the low level
   assembler code?
  * Relatable...[wanting to make some small modifications but getting blocked
   from doing it because of underlying
   complexity](https://news.ycombinator.com/item?id=12817468)
  * [Feedback, consistency, visibility](https://news.ycombinator.com/item?id=12822115)
  * [Stuff People Use to Get Software to Run](https://web.archive.org/web/20170222150103/https://gist.github.com/ibdknox/8f15441530bdd09aa8ce489dd9c110c7)
  * [Postmortem of Eve and
   LightTable](https://observablehq.com/@jashkenas/against-the-current-what-we-learned-from-eve-transcript)
* [Eve Semantic Wiki](https://www.youtube.com/watch?v=VZQoAKJPbh8&feature=youtu.be&t=46m20s)
  * Nothing new under the sun: [SPARQL](https://www.w3.org/TR/rdf-sparql-query/)
  * Is the [wiki like overlay](https://news.ycombinator.com/item?id=12819514)
  what could really be the killer feature from Eve?
* [Hypercard: The Software Erector Set](https://hypercard.org)
* [If This Then That (IFTTT)](https://ifttt.com/explore)
  * Looks like Zapier but with simpler semantics.
  * Nothing against making it easier for people to link up tools they like.

__Better Programming With Existing Tools__:
* [Aspect Oriented
  Programming](https://stackoverflow.com/questions/242177/what-is-aspect-oriented-programming)
  -- [Cross Cutting
  Abstraction](https://en.wikipedia.org/wiki/Aspect-oriented_programming#AspectJ's_join-point_model)
* [Reduce Cpp Compilation Time](https://codingnest.com/the-little-things-speeding-up-c-compilation/)
* [Cpp Linkage Rules](http://www.goldsborough.me/c/c++/linker/2016/03/30/19-34-25-internal_and_external_linkage_in_c++/)
* [Homoiconicity](https://news.ycombinator.com/item?id=12819585)
* [Monoliths vs Microservices](https://news.ycombinator.com/item?id=22193383)
  * I think I'm missing the experience to really understand some of the points
  being made here.
* [Distributed (Networked) Programming is
  Hard](https://news.ycombinator.com/item?id=23212573) : [fragile, narrow,
  laggy, async, mismatched, untrusted,
  pipes](https://thume.ca/2020/05/17/pipes-kill-productivity/)
  * I learned what
   [HashDOS-ing](https://www.anchor.com.au/blog/2012/12/how-to-explain-hash-dos-to-your-parents-by-using-cats/)
    is.
  * [HTTP/2 Server Push](https://en.wikipedia.org/wiki/HTTP/2_Server_Push)
    helps to alleviate performance issues by preemptively sending resources.
  * Also [Kafka](https://kafka.apache.org/) for syncing.
  * Love [this comment](https://news.ycombinator.com/item?id=23216914) despite
    the lack of grammatical parallelism: "having
    what you need, when you need it, where you need it, and understanding how
    to use it."
  * Also [yes Erlang](https://news.ycombinator.com/item?id=23213438) if you can
  * Sometimes you should just [do something simple](https://news.ycombinator.com/item?id=23212787)
    * Besides, not all of us are [building multi-million dollar, multi-million
   user cathedrals](https://news.ycombinator.com/item?id=23215224).
* [Tristan Hume](http://thume.ca/) seems like a smart boy that knows much more
  about programming than me, so I figured I'd [read some more of his
  work](https://blog.janestreet.com/commas-in-big-numbers-everywhere/)
  * The fact that you can make a [font that automatically renders into tiny
  charts](https://aftertheflood.com/journal/the-worlds-first-code-free-sparkline-typeface/)
  is blowing my mind.
* [Human Filtered Common Postmortem Failure Reasons](https://danluu.com/postmortem-lessons/)
  * As usual, Dan's writing is completely brilliant and worth reading as many
    times as it takes for you to get the point and maybe actually do what he
    suggests.
  * Here's the [Jepsen series](https://aphyr.com/tags/jepsen) if you're still
  interested in pulling on this thread.
  * Error Handling -- [92% of critical, cluster-taking down or data corrupting,
   failures n Cassandra, HBase, HDFS, MapReduce, and Redis were the result of
   bad error handling](https://www.usenix.org/conference/osdi14/technical-sessions/presentation/yuan).
  * Configuration (I've caused my fair share of these issues).
  > it's not so obvious that most companies test and stage config changes like
  > they do code changes
  * Hardware. Advertised failure rates are not necessarily as accurate as they
    should be. Error detecting hardware isn't necessarily reliable.
  * Humans (process errors)
  > if you repeatedly put a human in a position where they can cause a
  > catastrophic failure, you'll eventually get a catastrophe
    * How underrepresented is this problem? It's certainly insidious. It's also
      definitely embarrassing to admit to.
    * Computers happen to be pretty good at doing something exactly to
      specification.
  * Monitoring / Altering
    * You can't rely on ops heroism to save your day!
  * Eyo, obvious doesn't mean it's been taken care of. Good Lord, how many
    times do I read something and think "that's so obvious. This person just
    put the words together in a better way than I could". Oftentimes, spending
    a little more effort questioning whether those things that you say
    "obviously" or "of course" to are actually handled in the "obvious" way can
    save you immense amounts of headache in the future.
* [What is DVC](https://news.ycombinator.com/item?id=19129408)
  * [DVC vs other technologies](https://dvc.org/doc/user-guide/related-technologies)
  * [Symlink vs hardlink vs reflink](http://www.pixelbeat.org/docs/unix_links.html)
   for [DVC](https://dvc.org/doc/user-guide/large-dataset-optimization)
* I still don't really understand it, but I suppose I can bookmark it here in
  case I ever need to write a [DSL](https://www.jetbrains.com/mps/).

__Computing History__:
* [MVC (Model View
  Controller)](http://heim.ifi.uio.no/~trygver/themes/mvc/mvc-index.html)
  > The essential purpose of MVC is to bridge the gap between the human user's
  > mental model and the digital model that exists in the computer.<br>---<br>
  > MVC was conceived as a general solution to the problem of users controlling
  > a large and complex data set.

__Cool Software Projects__:
* Ray Tracing @30FPS in
  [Notepad](http://kylehalladay.com/blog/2020/05/20/Rendering-With-Notepad.html)

__Managing Software Projects__:
* [90% of Programming is Under the
  Water](https://www.joelonsoftware.com/2002/02/13/the-iceberg-secret-revealed/)
  * What non programmers (or the client in general) see is the UI. UI looks bad,
  the project clearly is in a bad state. UI looks nearly done, the project
  clearly is almost done.
    * Let the client play with various designs (just like your house designer
      lets you play with color swatches and make other cosmetic decisions) so
      they feel important.
    * When you do a demo, make each component look in accordance with its status
    on the backend. Finished stuff should look fantastic; unfinished stuff
    should look correspondingly rough around the edges. In fact, you might
    consider excluding unfinished stuff so people can't nitpick about it.
  * Don't forget to [control what people think about the
   schedule](https://www.joelonsoftware.com/2007/10/26/evidence-based-scheduling/)
    * Break down the schedule into steps that are each no more than 16 hrs long.
    * Track estimated vs actual hours spent on a task and use the historical
      data to adjust the schedule.
    * Use Monte Carlo simulation to build a CDF for ship dates.
    * Now manage the projects to account for uneven workloads and uneven
      forecasting abilities. Plot the ship date confidence intervals against
      each other so you can track trends in how ship date is shifting.
      * The person doing the work is responsible for creating the time estimate.
      * Fix bugs as you find them and extend the schedule once the bug arrives.
        After a few iterations of this, you'll know how to adjust the schedule
        to get at the time estimate for fully debugged code.
      * Time pressure doesn't work! Don't let managers try to pull progrmamers
        behind schedule as a way to motivate them.
      * Remember the [iron
        triangle](https://en.wikipedia.org/wiki/Project_management_triangle).
        You can cut scope or move the schedule out. You probably want to cut
        scope and force focus onto the essential features.

__Specks of Dust that Keep Flying Into My Eye__:
* I get very upset at people who aren't able to evaluate the quality of their
work for themselves. To be honest, it probably took me until junior or senior
year of college before I could confidently make statements like "this is a 'B'
paper" (and yes it was only in the context of writing). It's not like I never
knew the quality of my writing. I just didn't have writing that was above my
threshold of quality until I hit college. Anyway, once my internal barometer
got tuned, and I began thinking harder about false respect for authority
like teachers and indoctrination for a limited set of subjects that is school
and the school curriculum and how school exposes you to such a small number of
pathways towards financial sufficiency (because we all know that success is not
defined by money but that financial self-sufficiency is a pretty good place to
be in), I just became so angry and shocked at all the ways we'd suppressed
people's internal senses for quality. You don't need someone to tell you whether
you're good or not. Ah, more on this once I read [this
book](https://www.amazon.com/Punished-Rewards-Trouble-Incentive-Praise/dp/0618001816).
  * [Rewards and punishment are behavior manipulation
   tools](https://www.alfiekohn.org/article/punished-rewards-article/). Would
    anyone like to argue against the idea that schooling is anything but an
    institution designed for the molding of docile and obedient and rigid
    behavior? What's especially insidious about these tools is how often the
    distance between the initiating behavior and the reward or punishment exceeds
    anything that naturally could occur as a consequence. Why does it make sense
    to use a desire for something like pizza as the lever for encouraging good
    performance on a test (tests are pieces of crap, too, but let's get to that
    later)? Why does it make sense to use a desire to avoid something like social
    isolation (not being allowed to see your friends this weekend) as a lever for
    preventing or retaliating against something like trekking mud into the house?
    * Rewards and punishments are also complete motivation killers. There's
      nothing more beautiful about people than intrinsic motivation or curiosity.
      Rewards and punishments are tools for compliance that basically say
      "whatever you're interested in is unimportant because [it's inconvenient to
      me right now] OR [it upsets me in some way and I have authority over you
      (for some other arbitrary reason)] so take this candy as reward for
      temporarily suppressing your internal compass in favor of my direction".
      Of course, the temporary suppression is anything but temporary.
    * This comes back to my previous point about how you [can't convince people
   of anything](../../01/02/important-skills-html). Environment and incentives
   are the key inputs to any function of behavior. Too bad we often design those
   things to encourage stamping out the human spirit.
* The best way to exercise self control is to not need to exercise it at all.
  Get yourself out of triggering environments (and maybe reexamine your
  triggers).
* Full employment is just keeping everybody busy (doing stuff other people told
them to do).
* I've actually had this one for a while. I just didn't know where to put it or
whether I was going to expand on it: "No one likes being treated like a child."
* When POPULATION has MOTIVATION, and LIMITATIONS, they will BEHAVIOR as
  measured by DATA.
* Data cleaning / ETL should be separated from your BI tool (Jon Avrach 2019)
* One-on-One Questions:
  * What have we done well / need to improve in the last year?
  * What do you feel is blocking our productivity?
  * What could level up the team?
  * Knowledge transfer. What productivity information or company information is
  it important for team members to understand?
  * What decisions have you made that have had the biggest impact on your
    career.
* TS Context Specific Projects
  * Knowledge graph.
  * Mixed media publishing tool.
  * Graph / network exploration.
  * Alternative search engine suggestion ranking.
  * State exploration for Explore so you can click on bubbles to go back to any
    previous state.
