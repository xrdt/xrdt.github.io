--
layout: posts
title: "The Rising of August"
---
*Author: Bianca Yang*<br>
*Email: <a href="mailto:ipacifics@gmail.com?subject=Hello from the XDRT Blog">ipacifics@gmail.com</a>*<br>

These monthly files have been a great way for me to keep track of and actually
reflect on my reading. The problem is that I'm a lazy butt and categorizing all
my links and even building a table of contents to make navigating this mess of
links and notes is beyond what I care to be doing right now. I will shift to
weekly compilations for September and see if that improves anything about this
public journal blog format.

__Unconnected Thoughts__:
> Ask for what you want. It's their job to turn you down, not yours.
> [If you've never been scammed, your baseline level of trust in people is too
low](https://www.scottaaronson.com/blog/?p=40).
* [Definition #4 of Essay](https://en.wiktionary.org/wiki/essai)
* I've found that during technical interviews, when people ask me leading
questions, like "why don't you think about count", my thinking gets
short-circuited. Of course, this is not unique to me. I've noticed it in people
I've interviewed, too. Clearly the suggested solution is superior to whatever
backwards nonsense track I'm letting my brain wander free along so I should just
stop everything and narrow my focus on the few tidbits they gave me until that
tidbit glows red hot from the intensity of my mental gaze. Is the tip effective?
Hard to say...if I already have what they're thinking about in my current search
buffer I can readily return a "yeah but I'm also thinking xyz". If I don't have
anything near what they're suggesting in my current search space...it's not
necessarily super effective. In fact, the mental effort required to rejigger
my thinking to accommodate their suggestion is so much that it might just blast
through any productive whisps of thoughts I was having. Maybe it's more
effective to ask the person what they're thinking and then give a few examples.
Hm, how do you help someone who's stuck without giving them the answer or
stopping their train of thinking.

__Books and Treatises__:
* [To Pixar and Beyond](https://www.amazon.com/Pixar-Beyond-Unlikely-Journey-Entertainment-ebook/dp/B01912OSA0)
  * In this book, former Pixar CFO recounts his journey with the now hallowed
  computer animation company. He starts with his first phone call with Steve
  Jobs about joining the company and takes us through the company's hot 1995 IPO
  to how he negotiated equal profit sharing on the movies and equal branding on
  the merchandise with Disney to the 2006 acquisition by Disney. It's an easy
  and enjoyable read, something you wouldn't regret having packed in your
  suitcase before you headed out to Cabo for a summer getaway.
* [Richard Gabriel on Why OOP Has Failed](https://www.dreamsongs.com/Files/ObjectsHaveFailed.pdf)
  * OOP is a totalizing paradigm (objects represent how objects work in the real
  world; everything is an object) that has serious flaws with being too static
  (not resilient, easy to break interfaces). We need to encourage diversity of
  thought about programming (functional, data driven, logic, expert systems,
  etc.) so we can continue to push forward how humans interface with computers.
    * Think about the fact that Go4 patterns could be easily implemented in
    Lisp using first class constructs.
    * OOP promised reuse but that turns out to be very hard to manage the
    operations. It's cheaper mentally and time wise to just rewrite things by
    yourself.
    * Encapsulation has failed because things like errors and performance aren't
    encapsulated within objects. OOP also makes it hard to manage things like
    global consistency (think of singleton objects). If you do encode some
    synchornization mechanism for global consistency, you've just broken
    encapsulation and made everything dependent on everything else.
    * It's impossible to lay down a strict design up front for how all the
    objects in a system should work together. The psuedo mathematical or even
    factory manager derived rigor that Charles Babbage and Dijkstra encouraged
    has infected the field with a false sense of ability to define types or
    other static constructs that can represent and encompass the breadth of
    all things humans could want to build. Types can be too restrictive. Types
    were designed for ease of formal verification, not for ease of
    expressibility.
    * OOP designed systems do not evolve very well. Rewrites and bloat often
    occur because the langauges lack dynamism.
    * Databases, with their primary focus on separating state and behavior,
    cannot play well with OOP out of the box. OOP is focused on encapsulating
    bits of state and behavior into objects.
    * RPC -- it's not great to distribute a bunch of fine grained objects. Round
    trip times will always be slow. People decided to build XML and send massive
    objects in one go. This is how RDBMSs work.
    * Modeling Languages -- This is where OOP has really contributed something
    fascinating. Structure can be coded automatically while complex business
    logic will be coded by hand and plugged into the structure.
    * No need to go so far down the postmodernist rabbit hole and pursue
    totalizing paradigms. It's much better to find a way to have multiple ways
    of working integrate and contribute towards the same solution.
  * Programmers often wax poetic about how natural systems like the human body
  are able to coordinate actions among massive numbers of unreliable,
  independent entities. How can we get human written code to function with that
  level of robustness and ability to self-sustain? (Ref autonomic computing)
  * I'm not able to find a recording of the talk, but the introduction for
  [why objects haven't
  failed](https://www.dreamsongs.com/ObjectsHaveNotFailedNarr.html) is still on
  the internet.
    * The claim that OOP is successful because of wide adoption is weak.
    * OOP works on the premise that "smart data structures and dumb code works
    better than the other way around".
    > Show me your interfaces, the contracts for your methods, and I won't
    usually need your field declarations and class hierarchy; they'll be
    irrelevant.
      * Does OOP resolve the concerns of ongoing programs, like the ones
      being deployed on the World Wide Web, better than functional or procedural
      programming?
    * Well, this author acknowledges that OOP isn't perfect. He's merely saying
    that there's lots of evolution from the early days of Smalltalk based OOP
    and that we do have to consider where each tool (functional, procedural,
    object-oriented) best fits into the larger programming ecosystem.

__Cool New Tools__:
* [What If Tool](https://pair-code.github.io/what-if-tool/get-started/) for
exploring ML models.
* [Embedding projector](https://projector.tensorflow.org/) from Tensorflow.

__Raw Internet Links__:
* [Have You Thought About Compiling Your Personal Canon Yet](http://davidcole.me/canon/)
* [It's Not Like Spelling Things Over the Phone Has Ever Been Easy](https://www.mcsweeneys.net/articles/e-mail-addresses-it-would-be-really-annoying-to-give-out-over-the-phone)
* [It's Been a Long While Since I've Read Short Fiction](https://www.newyorker.com/humor/daily-shouts/sell-out-part-one)
* [Jane Street Pay](https://news.ycombinator.com/item?id=24272514)
  * You can make 7 figures, but you gotta prove you're worth it. It's easier to
  get to a point where you're making 7 figures if you start out early and growth
  within the company than if you join as a senior person.
* [Apple is Figuring Out How to Break Free of the iPhone](https://stratechery.com/2019/apples-audacity/)
  * This was written in June 2019. It was clear that iPhone growth had plateaued
  and the contribution of the iPhone to revenue was decreasing. Rather than
  focus more on ramping up internal revenue generators by increasing prices,
  Apple has been looking to expand new opportunities, like breaking up iTunes
  into Podcast, Music, and TV; making the Apple Watch independent with its own
  app store; and introducing the iPadOS branding. The company is also pushing
  forward on its commitment to privacy with "Sign In with Apple". The end result
  here is similar to what [privacy.com](https://privacy.com) and
  [Abine](https://www.abine.com) have done: obfuscate emails to subvert data
  collection efforts.
  * There's also a blurb at the beginning about the Mac Pro being an audacious
  tech statement in the way that supercars are an audacious tech statement.
* [Response to Andreessen's piece on the Time to Build](https://nintil.com/on-building/)
  * Things are being built. They just aren't being built fast enough. How do we
  remove regulatory friction so people will be incentivized to build rather than
  collect their golden handcuffs paychecks at fancy techbro companies? If
  companies and institutions eventually accumulate enough crud that slows them
  down, how do we build in replacement mechanisms so fresh blood and thinking
  can come in and deliver the needed, if not desired (want a faster horse?),
  innovation?
* [Why America Doesn't Make Things Anymore](https://americanaffairsjournal.org/2019/05/financing-advanced-manufacturing-why-vcs-arent-the-answer/)
  * VC isn't incentivized to invest in anything besides pharma and software.
  Hard tech innovation and manufacturing is all moving overseas because it's
  easier to acquire funding, especially for expansion there. It used to be that
  hardware companies could acquire large amounts of financing through IPOs or
  acquisitions. Now, the IPO market has dried up and major US manufacturing
  companies have largely outsourced manufacturing to Asia.
  * We used to think that only low level manufacturing was outsourced to Asia.
  Now it's becoming evident that even advanced manufacturing is moving offshore.
  * Other countries like Britain experimenting with special government funds for
  manufacturing. Israel and Germany have made it favorable for commercial banks
  to lend to manufacturing startups looking to scale up. In Israel, the
  government guarantees the loans.
  * The right doesn't like government intervention. The left can only accept
  increased manufacturing when it's tied with environmental interventions and
  social justice. No clear policy that will be accepted in America but we do
  need some way to get building back on American land.
* [Brent Beshore Fishing for Investment Ideas](https://twitter.com/BrentBeshore/status/1283119266691153923) (I'm screwing around with the "fishing for" phrasing.)
  * [Alex Danco's take on Canadian REITs with hardy tenants like Walmart](https://twitter.com/Alex_Danco/status/1283123882078109696)
    * [Chamath said he was looking into REITs with similarly hardy tenants in April](https://www.businessinsider.com/chamath-palihapitiya-shares-3-part-investing-strategy-for-coronavirus-market-2020-4)
* [So There's Some Correlation Between Length of Chinese Names (1 vs 2 Char) and End of Dynasties](https://twitter.com/yiqinfu/status/1298437372284211200)
* [Japan Remastered 1913 - 1915](https://www.youtube.com/watch?v=MQAmZ_kR8S8)
* [Sin taxes on sugar didn't work in Philadelphia](https://twitter.com/bansisharma/status/1083714031339401218).
  * Taxes disproportionately affect the poor, who are less likely to go to
  another, nearby city for untaxed goods. The government also views taxes as a
  revenue stream and builds it into future budgets. This creates revenue
  problems because, if these sin taxes decrease, the government will have a lost
  a portion of revenue it foolishly came to depend upon. Taxation should be
  applied as broadly as possible, to avoid gaming of specific rules.
  * Only cultural change (stigma) and public behavior enforcements (no smoking
  areas) and education can break society wide addictions like smoking and sugar
  consumption.
* Good Lord the Bay Area is [covered in lava](https://twitter.com/CALFIRECZU/status/1297383648065249280)
* A Beautiful [Love Story](https://lemobilefeast.com/2020/08/23/a-love-story/),
written by a former high school teacher who later embarked on a 3 year mobile cooking and story collecting journey
* Words on StitchFix [straight from the CEO](https://hbr.org/2018/05/stitch-fixs-ceo-on-selling-personal-style-to-the-mass-market)
* [Rene Girard Quotes on the Apocalypse](https://medium.com/@ryanpflynn/rené-girard-battling-to-the-end-quotes-891b535b43ed)
* [Bill Gurley on What Characterizes Strong Revenue
Streams (2011)](http://abovethecrowd.com/2011/05/24/all-revenue-is-not-created-equal-the-keys-to-the-10x-revenue-club/?ck_subscriber_id=547821799)
  * People like Price / Revenue ratios and DCF but not all revenues are the same
  and DCF is notoriously difficult to get right. There is huge disparity in P/R
  ratios, from 0.2x for Overstock to 21.7x for YouKu (2011). What figures?
    * Moat. Durability of competitive advantage.
    * Network effects. What is the decay function for the marginal contribution
    of each new user to the platform? Know the difference between returns to
    scale and network effects.
    * Predictability of revenues. Subscription vs. one time.
    * Switching costs and customer lock in. Talk to me about that churn.
    * Gross margins.
    * Marginal profitability: change in revenue / change in costs. Is this
    number improving?
    * Customer concentration. Diversity in customer base.
    * Partner dependencies.
    * Organic demand vs marketing spend.
    * Growth. Watch for companies substituting revenue growth for profits
    (selling dollars for cents) or riding a trend that has little to no
    barriers to entry.
    * Capital expenditure intensity.
    * Optionality (AWS opening up revenue streams for Amazon).
    * Cash flow / earnings. Cash is king.
  *  [The New Increasing Returns Paradigm of Firm and Product Maturation
  (1996)](https://hbr.org/1996/07/increasing-returns-and-the-new-world-of-business)
    * The old economic paradigm has been dominated by an assumption that world
    operates on diminishing returns. A (stagnating?) equilibrium will eventually
    be reached. This is a view of the world that fits the standard company of
    the Industrial Revolution: bulk-manufacturer whose growth is limited by
    access to resources.
      * The priority for these bulk processing companies is to make sure there
      is no break in the supply chain. Their bread and butter is control and
      planning and optimization of those functions. Hierarchical structures
      dominate.
    * Knowledge based industries tend to be governed by increasing returns
    and positive feedback loops.
      * Think winner take all markets. Rich get richer and the poor get poorer.
      Ecosystem lock-in. Fat profits for the winner. Inferior
      product that gets the market to tilt in its favor may win.
      * Management here is constantly focused on looking for the next big
      winner. They're always looking around the casino, trying to decide which
      tables they want to gamble it. Hierarchies flatten because the next big
      thing can come from anyone in the org. It's not a management game for the
      faint hearted. Adaptation and nimbleness must be your main competitive
      strengths.
      * How do you win in this game?
        * Heavily discount initially to acquire users.
        * Build a 2-3x(sic) better product.
        * Build an (cross-company) ecosystem with network effects.
        * Play the psychology of convincing others that a market is already
        locked in to prevent others from attempting to compete.
      * When locality doesn't matter, winner takes all will dominate.
      * When locality does matter, smaller local players will tie into a central
      network, like law firms tied to Lexis-Nexis or doctors tied to HMOs.
    * Why is high tech dominated by increasing returns:
      * Up front costs and decreasing marginal costs.
      * Network effects.
      * Customer lock in.
    * Play the increasing returns game well:
      * Watch the feedback loops
      * Watch the ecologies you play in
      * Do you have the resources needed to make the right sized bets?
      * What's on the horizon?
    > As the economy shifts steadily away from the brute force of things into
    the powers of mind, from resource-based bulk processing into knowledge-based
    design and reproduction, so it is shifting from a base of diminishing
    returns to one of increasing returns.
* [The ideal mobile base of operations vehicle HNews style](https://news.ycombinator.com/item?id=23704497)
* [The 2010 shape of Science](https://pasteboard.co/JkLvTsI7.png)
* [Gaming the system -- Chinese Virus Style](https://twitter.com/calebwatney/status/1243564258757160967)
* [In case you thought jobless claims in 2020 weren't too crazy](https://twitter.com/lenkiefer/status/1243166718924554240)
* [Nietzche Truth and Lies in a Nonmoral Sense](http://nietzsche.holtof.com/Nietzsche_various/on_truth_and_lies.htm)
  * I'm not sure what I got out of this. More thinking needed.
* [Bytedance Self Regulation of Live Video Streaming Platforms White
Paper](https://gofile.io/d/hGmt9C)
  * This [Twitter
  thread](https://twitter.com/izzy_niu/status/1280906441654747136) gives a good
  summary of the contents.
* [SQL Tutorial 1](https://quip.com/2gwZArKuWk7W)
  * [SQL Tutorial 0](https://selectstarsql.com)
* [Erik Torenberg Compilation of SSC Ideas](https://twitter.com/eriktorenberg/status/1244051290100920321)
  * [Proving Too Much](https://en.wikipedia.org/wiki/Proving_too_much)
  * "Universalize as if the process you use to universalize would itself become universal."
  * "But there’s a risk that postmodernism collapses into ppl ignoring any facts
  they disagree with, arguing that facts are mutable products of hostile power
  structures trying to perpetuate themselves. And by 'there’s a risk', I mean
  'this has been obviously happening for decades'.
  * "Postmodernism says that facts often get reframed to support the powerful.
  So it’s inevitable that post-modernism itself going to be twisted to support
  the powerful. (e.g. both cultural Marxists, & far-right media)."
  * If you trust Alexey Guzey's curation judgement, you can also read his
  collection of [favorite SSC posts](https://guzey.com/favorite/slate-star-codex/).
* [Scrappy Building in Tough Times](https://elizabethyin.com/2020/04/11/operating-in-tough-times/)
* [Primer AI's (NLP Startup) Auto Generated COVID Dashboard](https://covid19primer.com/dashboard)
  * Met the guy who [built this](https://denread.com/) on Lunchclub the other
  day. He's now thinking about building a similar, nearest neighbor paragraph
  search tool. Below are some other cool tools that he introduced me to.
    * [AI powered scientific search engine](https://www.resolute.ai/how-it-works)
    * ["Automated" Information Extraction from Arbitrary
   Documents](https://www.infrrd.ai/). I put quotes because apparently a lot of
   the work is manual labor.
    * [Google Alerts](https://www.google.com/alerts). Good old keyword based
    web monitoring. It will probably take some time to get the keyword search
    to have the right recall and precision, but it seems like a nice way to
    escape the black holes that explicitly algorithmic suggestion feeds
    inevitably turn into.
* [250 Things an Architect Should Know](https://www.readingdesign.org/250-things/)
  * Origin: Michael Sorkin
  * Reality is more complicated that you think it is.
  * There's always more to learn.
* [How Coronavirus Accelerated Technological Developments May Rewrite our Cultural Map](http://subpixel.space/entries/premonition/)
  * How will culture shift online? Probably micro networks will explode. People
  can't handle all the mainstream social networks. Intangibles like activities
  and narratives will take precedence. Knowledge tooling will evolve to support
  the new ways to share units of cultural significance.
  * Brands with relationship models will hold up better than ones like
  dropshipping and other low-margin microbrands. How will DTC work without
  infinite VC funding? People like participating in the success of brands so
  crowdfunding and patronage will probably accelerate.
  * People will not be nearly as comfortable being in dense urban spaces as they
  were before (seems like a very American phenomenon, given how undense most of
  the country is). Who will now vacant ground-floor real estate in prime urban
  streets go to? The small entrepreneurs or the big box players like Amazon?
  * More entertainment, less money to get it. People are going to get creative
  to satisfy their needs.
  * How can tools like Zoom (and nascent competitors like Roblox/) help people
  better structure their time? Watch for the emergence of spatial interfaces.
  * Eyo will people ever die? Given that you can create deepfakes of anybody
  with a sufficient online presence, how will you send people off? When will
  you do it? Or will their computer supported consciousness meld into the
  backbone of the web?
* [Exploration of the End of Authenticity](https://subpixel.space/entries/after-authenticity/)
  * It's not longer selling out to capitalize on your reach and get famous and
  break out of indie / hipster circles.
  * Authenticity also exists in tourism and anthropology circles. We want
  authentic native or tribal experiences. We don't want some trinkets that were
  manufactured for the Westerners seeking to take some memento of their time in
  a foreign place home. We want the original object, untouched by capitalism,
  raw and inherently useful in the local context.
  * 20th century African art fetish:
  > African art picked up randomly in the course of fieldwork was placed
  entirely in a closed sphere with a sacred cast. [...] It was not considered
  entirely proper to acquire an art object from African market traders, or
  worse, from European traders in Africa, or worse still, from dealers in Europe
  or America.
  * 2008 Hipster music: “you probably haven’t heard of them”. If you have,
  they're a sell out. Of course, this extended to everything else that could
  define an individual: fashion, food, accessories, films.
  * One theory is that authenticity culture emerged out of the economic
  uncertainty of the 2007 - 2008 financial crisis. Maker movement and indie
  entrepreneurism also emerged out of the need to make one's own economic
  future.
  * Authenticity is now a marketing term that can get thrown on any modern items
  to give it a bit of that nice antique patina. We've figured out how to scale
  authenticity (single-lot, artisan, hand-crafted, etc). Ref Venkatesh Rao's
  [premium mediocre](https://aeon.co/essays/america-still-has-a-heartland-it-s-just-an-artificial-one)
  [essays](https://www.ribbonfarm.com/2017/08/17/the-premium-mediocre-life-of-maya-millennial/)
  Call it "contemporary conformism", as Carles does. Or maybe you like
  "authentic consumption".
  > Auth music doesn’t really have a wide-reaching sound. It is not ‘scalable.’
  Auths do not have a visual aesthetic like ‘hipsters.’ Auth is a state of mind
  where you cannot be influenced. U can only vibe and approach the world with an.
  auth state of mind. No brands represent u.
  > The history of 21st century authenticity is the history of hipsters and
  their disappearance.
  * How can you think outside of authenticity politics?
  * [Brandless](https://brandless.com/)???
  > [W]e need more nuanced forms of critique that address how brands participate
  in society as creators and collaborators with real agency. ... Brands
  and commodities therefore need to be considered and critiqued on the basis of
  the specific cultural and economic contributions they make to society.
  * Brands are a substrate for meaning and individual differentiation.
* [Umami, Premium Econmy, Excess Meaning, Death of Experience Economy](https://nemesis.global/memos/umami)
  * Written in March 2020.
  * Spending on experiences was the pre-corona standard of premium consumption.
  * People high on the promises of unlimited, endless meaning making in the
  experience economy wanted umami. Umami is what you got when you didn’t get
  anything.
  * Financialization (2008 - 2018) -- "What was actually happening was the
  enrichment of financial assets over the creation of any ‘real wealth’ along
  with corresponding illusions of progress". Little to no physical investment.
  Little to no new physical goods development. All that's left is repackaging
  of the immaterial --> hence distilling our world into it's most savory and
  umami pieces.
  * What is umami: "SYNERGY, IMPRESSION OF THICKNESS, and PARTS > WHOLE"
    > “This shouldn’t be good but it is”

    > “This doesn’t seem like what it’s supposed to be”

    > “This is both too much and not enough”

    > “I shouldn’t be here but i am”

    > “This could be anywhere but it’s here”
    * ^ in a temporary but consciousness encompassing flow of experience
    thickening (could be paradoxical)
    * People can't keep up with the umami experience generation machine and
    think deeper about the fact that there's no meaningful substrate underlying
    these pieces of yummy, fun, obviously temporary sensory heightening memes.
  * How do you create meaning when anybody can reorganize the existing meaning
  graph (infinite free money)? You create feelings of scarcity. You make things
  that only the in group can "get".
  * What's next? No one knows. But our minds and feeds are saturated with this
  frothy nonsense that has made our lives interesting for the past X years.
  Something else must emerge to satisfy our desire for distraction and
  differentiation.
* [Spatial Interfaces--Basically when Building Digital 3D Experiences Makes More Sense than Building 2D Ones](https://darkblueheaven.com/spatialinterfaces/)
  * Reducing dimensionality doesn't always make designing and programming
  digital experiences easier. It's far more difficult to program a generic
  deck of cards for any kind of game than it is to build a generic 3D deck of
  cards.
  * Why now? Gaming has been the leader in 3D experiences and the developments
  there are permeating other folds of society through digital 3d places like
  Fortnite and e-sports. The tools required to create 3D experiences have become
  much, much easier to use and available in a much larger variety of programming
  languages and platforms. It's only getting easier to be a 3D developer.
  * Why are spatial interfaces important? Spatial interfaces are highly
  untuitive and information rich. It's how we navigate our regular environments.
  Skeumorphic design and Snapchat all provide spatial affordances to make the
  in-app experience more intuitive and rich.
  * The author proposes a way to leave a breadcrumb trail across the internet
  that I find reasonably interesting. It's basically a replay of how people
  traversed a series of web pages. His other suggestions are more "obvious", in
  the sense that they are skeumorphic 3D experiences. Think about holding
  conferences in a 3D avatar driven platform like Second Life or using a virtual
  office like Sococo.
* [In Case you Wanted a Nice Table to Share in Your Substack Newsletter About
How the World has Changed](https://marginalrevolution.com/marginalrevolution/2020/04/world-2-0-there-are-decades-where-nothing-happens-and-weeks-where-decades-happen.html)
  * [No way out of commodity culture](http://www.shaviro.com/Blog/?p=394)
    * [Referenced book](https://www.amazon.com/exec/obidos/ASIN/0060935235/dhalgrenstevensh)
* [Resolute Optimism](https://resoluteoptimism.bailliegifford.com/) -- A
Different Take on How to do Investing Properly
* [Very Impressive Nike Commercial](https://www.youtube.com/watch?v=WA4dDs0T7sM&feature=youtu.be)
* [Brilliant Awk Script for Calculating Shared Expenses](https://c2.com/doc/expense/)
  * I love awk. This script took me some time to parse, but once I got it, bam!
  lightbulbs flashed in my mind.
* [The Biggest Ed Psyc Resources Compilation I've Seen So Far](http://www.edpsycinteractive.org/materials/videos.html)
* [Elon Pushing the Status Quo as Usual](https://threadreaderapp.com/thread/1292818184588886016.html)
  * Story about Tesla IPO and Elon being a maverick.
* [T-Cell Immunity and the Plateau of COVID Spread](https://twitter.com/JamesTodaroMD/status/1292873236716433416)
  * Basically only need 10 - 20% to be infected with COV-19 to get herd immunity
  b/c people have t-cell immunity from previous infections. Thus, any sheltering
  in place and mask wearing and otherwise infection slowing activities are just
  prolonging our adaptation to the virus and setting the right conditions for
  companies like Moderna to make bank on a vaccine.
* [Knowing this Distribution of Numbers can Help with Fraud Detection](https://economicthinkinginaction.com/benfords-law-and-fraud-detection/)
  * It is certainly not uniform. One occurs far more often than you'd see in a
  uniform distribution.
* [Some Good Advice on Thinking About Your Career and Companies to Join](https://www.reddit.com/r/cscareerquestions/comments/7u3cza/has_anyone_worked_at_a_biotech_company/dtixabp/)
  * I am really drawn to the widget / director distinction.
* [Spooky House. Look through All the Photos](https://my.flexmls.com/traviskempf/search/shared_links/3mADu/listings/20200812154502685559000000#share_link_modal)
* [Poignant Description of the Weather in Japan](https://twitter.com/craigmod/status/1295245710925824001)
* [Toby Ord Philosopher and CoFounder of Effective Altruism Movement on the
History of Thinking on Whether Mankind will Destroy
Itself](https://www.edge.org/conversation/toby_ord-we-have-the-power-to-destroy-ourselves-without-the-wisdom-to-ensure-that-we)
  * Referenced materials and people:
    * The Fate of the Earth, by Jonathan Schell
    * [Nuclear Winter, by Carl Sagan](https://www.cooperative-individualism.org/sagan-carl_nuclear-winter-1983.htm)
    * Reasons and Persons, by Derek Parfit
    * The End of the World, by John Leslie
    * Animal Liberation, by Peter Singer
    * John Broome
    * The Precipice, by Toby Ord
    * A 1900s lecture from HG Wells. Not sure which [one he's referring to](https://airminded.org/biographies/h-g-wells/)
* Tooling can always get better. This time [mathematical
diagramming](http://penrose.ink/siggraph20) is what is getting a facelift.
* [Report on how the Home Transforms As a Result of COVID Imposed Work from Home POlicies](https://www.yakcollective.org/projects/the-new-old-home)
  * The Yak Collective is a group of indie contributors. This is their second
  piece on how COVID will change our lives. The below list covers the points
  from the presentation that I thought were salient.
    * Home is moving towards coziness.
    * [Nuclear
   family](https://www.theatlantic.com/magazine/archive/2020/03/the-nuclear-family-was-a-mistake/605536/)
   and independent households disintegrate into coliving spaces
    ([it's](https://opendoor.io)
    [already](https://coliving.com) [happening](https://zeusliving.com)
    [everywhere](https://www.common.com/san-francisco/) you just need to be
    [looking](https://thehubhaus.com) in the [right places](https://topos.house))
    and intergenerational iving.
    * Move away from regimented and compulsory education for the young and back
    towards apprenticeships. This time, apprenticeships will be in the knowledge
    economy.
    * Everybody contributes meaningfully to chores, just like people did back
    when we lived on farms.
    * People need new tools to help facilitate new rituals to manage the
    distinction between work and life. Think Peloton or morning walks or morning
    espresso making or a daily Calm app session.
    * What will the future of family businesses look like?
* [SSC Reflection on His Intellectual Progress in the 2010s](https://slatestarcodex.com/2020/01/08/what-intellectual-progress-did-i-make-in-the-2010s/)

__China__:
* [A Perspective on Chinese Response to the Coronavirus Outbreak](https://www.newyorker.com/magazine/2020/08/17/how-china-controlled-the-coronavirus)
* [The Chinese Surveillance State (esp Xinjiang) and the Future of AI Safety in Surveillance Use Cases](https://www.theatlantic.com/magazine/archive/2020/09/china-ai-surveillance/614197/)
* [The Risks of Centralized Power, Re WeChat](https://twitter.com/yiqinfu/status/1299024297608896512)
  * [Chinese thread](http://weibointl.api.weibo.com/share/168796067.html) where
  someone basically says the issue is the intermingling of social and financial
  functions on the app. Posting content that is construed as sexual harassment,
  for example, should not prevent you from paying your bills or receiving
  business through the app. This is in response to an incident where a [young
  shopkeeper committed suicide after his WeChat account was
  frozen](https://outline.com/3PFKN8).
  * [When your WeChat account is permanently frozen (ahem excommunicated)](https://m.weibo.cn/status/4542579900685543#repost)
  I've translated the points below. Apologies for any glaring incompetencies in
  translation. My brain often shuts down to literal translation mode instead of
  thinking about how the contemporary English language is actually used.
    * #1 -- If you one day wake up to find that you automatically get kicked
    out of WeChat with a pop up window saying "This account is suspected of
    XXXXX illegal activity or rule violation and has been subject to permanent
    restrictions on logging in. Please hit 'enter' to see details.", do not
    panic! Things have already come so far. Panicking will do no good!
    * #2 -- Your account is permanently restricted from posting and editing
    information on the platform, including your personal information. Don't
    think you can edit your personal information as a signal to the outside
    world of your predicament. You should know that your account is now an
    informational black hole; you have no possibility of radiating out any
    information.
    * #3 -- You can still log in to your account through a "temporary login",
    but your activity is subject to the restrictions in #2.
    * #4 -- It is a false rumor that if you have taken out loans in WeChat, your
    account cannot be sealed. Your financial WeChat activity remains as is; it
    is merely your social WeChat that is blocked.
    * #5 -- You can still receive updates from groups you have joined.
    * #6 -- You can delete and leave groups.
    * #7 -- You cannot disband groups you have created. You can only leave those
    groups. You will need to find some way to communicate with the automatically
    chosen new group owner to delete the group you created.
    * #8 -- You can bind a new WeChat account to the phone number you were using
    with the sealed account. The sealed account will unbind from that phone
    number so you don't need to worry about your phone number becoming useless.
    * #9 -- You can't send WeChat contact cards to anybody.
    * #10 -- You cannot send QR codes for WeChat groups to anybody.
    * #11 -- You can create a new WeChat account but you will need to manually
    re-add all your contacts. If you can't find someone on WeChat through
    user-defined username or phone number, you two have effectively forever lost
    communications.
    * #12 -- You cannot join your original groups with the new WeChat account.
    You must find someone to invite you. (I'm not why it says original
    groups...can you join groups your sealed account wasn't part of??)
    * #13 -- If you've bound your WeChat to ETC (not entirely sure what this is,
    I think it's some way to pay traffic tolls), you can follow the public ETC
    helper account and try to switch the WeChat account your ETC is bound to.
    If you have a 2-wheeled ETC binding, then, congratulations, you cannot
    unbind your sealed WeChat account. Your ETC is now forever bound to your
    sealed WeChat account.
    * #14 -- If your WeChat has any no password required payment contracts, e.g.
    autopay Tencent Video VIP subscription, please cancel those subscriptions.
    Your WeChat account can no longer log into Tencent Video anymore.
    * #15 -- You are also forever unable to log into any Tencent properties
    that used the sealed WeChat account for log in. You need to manually unbind
    these accounts one by one. Some of these you will not be able to unbind.
    * #16 -- You can use another WeChat account to submit an appeal to customer
    support, but the success rate of the appeal is 0, 0, 0.
    * #17 -- Most likely your account was not sealed by WeChat. It was likely
    sealed because of XX circular. You don't know which deparment is responsible
    for XX. You don't have any way to submit an appeal for reconsideration. You
    don't even know concretely what you did wrong. It's all probability waves
    and black boxes permeating the space around you.
    * #18 -- Your sealed account will often receive messages from "WeChat Group"
    patiently reminding you: "You've already been sentenced to life
    imprisonment, stop the futile efforts to redeem yourself."
    * #19 -- WeChat is starting to do some canary testing of a new feature:
    extracting your communications logs from the app. It's not yet widely
    available.
    * #20 -- Don't put all your digital social interactions on WeChat. If your
    account is ever sealed, you will then have socially died.
    * #21 -- We need a new instant messaging tool.
    * A comment: No wonder the first step a lot of business people do after
    joining WeChat is leaving their phone number.

__Nutrition__:
* [Your Connective Tissues on Cake](https://crownmd.net/your-tendons-on-cake/)
* [Optimize Paul Saladino's Carnivore Diet](https://optimisingnutrition.com/optimising-paul-saladino-mds-nose-to-tail-carnivore-diet/)
  * [Paul Saladino](https://carnivoremd.com) is a voice of reason in the modern
  Twitter and podcast hosted debates on optimal nutrition. He's a big advocate
  for nose to tail carnivore and has successfully stuck to a no plant diet for
  about two years now. This post does an excellent job of breaking down Paul's
  micronutrient intake, explaining the relationship between calorie intake
  and intake of certain nutrients, and giving clear suggestions for how to
  improve intake of certain vitamins and minerals that Paul seems to be missing.
  Nutrition is the most interesting and fundamental field related to
  biochemistry and I'm so sad that schools don't include first principles,
  research paper based nutritional courses as a required part of the curriculum.
  Garbage in; garbage out, friends.
* [Fat vs Carb Oxidation and Storage in Active Individuals](https://sci-hub.tw/10.1139/h99-030)
  * Carb and protein preferentially oxidized. Fat initially shunted into adipose
  tissue. After about 4 days of high CHO diet, fat starts to be oxidized.
  Glycogen depleting exercise improves fat oxidation. Takes about 7 days to
  become fat adapted (fat burning). Sedentary people should therefore control
  their carbohydrate intakes because they can quickly oversupply their body's
  ability to store energy in muscle or liver glycogen or even in adipose tissue.
* [Carb Intolerance and Lipemia](https://sci-hub.tw/10.7326/0003-4819-68-4-926)
  * No connection between carb intolerance (diabetes) and lipemia (fatty acids
  in blood). Pretty much everybody has blood triglycerides go up 50-100%
  overnight after eating high CHO diet. Obesity is an aggravating factor in
  endogenous lipemia. Cellular adiposity leads to relative insulin insensitivity.
  Hyperinsulism is directly related to obesity and is also related to endogenous
  lipemia so obesity just makes the condition worse. Weight reduction again
  helps massively with the elevated serum triglyceride levels.
  Respect your insulin hormone!!!
* [Carb vs Fat Induced Lipemia](https://www.researchgate.net/publication/9706857_Carbohydrate-induced_and_fat-induced_lipemia)
  * Main focus on carb induced. Patients with fat induced, which is super rare,
  was due to severely lacking lipase enzyme activity (likely genetic). Not clear
  why carb induced happens but it was confirmed that the triglycerides in the
  serum were from lipogenesis from dietary CHO. For people with carb induced,
  lowest triglycerides achieved on high fat diets. Caloric insufficiency can
  also lower serum triglyceride levels. Very good research paper overall on
  how the body controls serum triglyceride levels.

__Podcasts__:
* [Chamath and Pomp](https://www.youtube.com/watch?v=_hA3TV1bGsg)
