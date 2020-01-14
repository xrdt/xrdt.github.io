---
layout: posts
title: "Some Color on ThoughtSpot Engineering"
---
*Author: Bianca Yang*<br>
*Email: <a href="mailto:ipacifics@gmail.com?subject=Hello from the XDRT Blog">ipacifics@gmail.com</a>*<br>

This is partly to document the current state of the system and to help candidates understand what they could be
getting into.

<u>The Five Engineering Teams</u>:<br>
* Falcon (our in-house database and manages data loading interfaces)
* Sage (search engine. Responsible for tokenizing input and turning input into intermediate SQL-like query. Also responsible for surfacing
completions as user types into search bar)
* Callosum (application server that manages connections between Sage -> Falcon and Falcon -> Blink. Also translates the output from Sage into
the database query language Falcon understands)
* Blink (front-end)
* Infra (they manage Orion, our cluster management system [we are moving to Kubernetes to enable more diverse deployments], Cloud, and everything
else)

How do all these components work together? Take a look at our [demo video](https://www.thoughtspot.com/product) first so you are grounded on our product.
The first point of interaction is with Blink, our front end team. Most data-related interactions (and which aren't?) you have with the front end will
first to go Sage, to parse the input. Some examples of interactions that go to Sage include: search bar queries and worksheet creation (basically custom
tables that users can create by pulling columns from any tables in the system. Once Sage parses the input, it will output an intermediate structured query
that can then go to Callosum for translation into TQL (ThoughtSpot Query Language, subset of SQL) for execution against Falcon. Once Callosum gets the
data back from Falcon, it will package and send it to Blink for display. Callosum is closer to the infrastructure than Sage and is also responsible for
things like chart generation (Callosum does basic templating but Blink makes the final decision about what fields to put on which axes and what chart type
is the most appropriate), managing lifecyle of objects like users, worksheets, tables, pinboards (our name for dashboards),
and data security and security groups. Our system is distributed, so Infra built Orion to manage communications between machines and is now facilitating
the transition to Kubernetes managed Docker containers. [Cloud deployments](https://docs.thoughtspot.com/latest/appliance/cloud.html) is another big
initiative that the Infra team is responsible for maturing. Falcon team is mostly responsible for making sure the database is highly functional and
keeping our data movement pipelines sharp, but it is now also responsible for [Embrace](https://docs.thoughtspot.com/5.3/data-integrate/embrace/embrace-intro.html),
our name for our initiative to expand the data sources we support. Embrace is a huge move for us because it removes major friction around loading data into
Falcon. Embrace allows customers to perform live queries against the database provider they are already using. We currently support Snowflake in beta but are
hard at work expanding into other major providers.

The company is heavily interested in cross-team collaborations, so we are often forming v-teams (virtual teams) composed of people across all teams (in many cases)
to push the product forward in interesting ways.

Interested in any of those groups? [email me](mailto:ipacifics@gmail.com?subject=Let's Talk ThoughtSpot) or connect on [LinkedIn](http://linkedin.com/in/yangbianca/).

<u>Quality of Work and Quality of People</u>:<br>
Choose who you surround yourself with carefully, because, like it or not, they will influence how you think, how you act, and who you
become. Choose to work in places that value craftsmanship and quality and (some level of) perfectionism. It will raise your bar to be around
people who produce at a high level.

It is hard to convince someone who has never interacted with our team or our codebase that we have excellent minds working on an amazing
piece of software. If you do come to do an onsite interview, I believe the quality of the team will shine through. If you look through our
codebase, you will realize that the foundational structures our core team of engineers who were responsible for building Bing, Google Borg
(which led to Kubernetes and Docker), massive infrastructure for delivering ads at Google and Amazon were extremely well engineered for
efficiency, extensibility, testability, and ease of use. This is undoubtedly a great place to learn the *craft* of software engineering and
will prepare you to build large scale, performant, and secure systems.

<u>What Makes ThoughtSpot's Product Unique</u>:<br>
There are a few hard problems in BI: data (dirty data, access to data), speed (complex queries with lots of joins take a long time), and skill set
(lack of technical skills among business users and lack of analysts with technical skills to help business users). ThoughtSpot has chosen to address
the latter two issues. We address speed with our in-house, read-optimized, columnar, in-memory database, Falcon. Trust me when I say that proper
ThoughtSpot can handle billions of rows in seconds. You'll be answering tens of questions with that saved time while your Tableau using buddies are
waiting for the spinning beach ball of death to resolve itself. One of our top sales engineers
(technical leader who helps with demos and proofs of value in early relationship building with the customer) said that the main reason customers pull
the trigger on a ThoughtSpot deployment is because of speed. Part of this is because the main buyers of our product are IT / Ops people. Those guys
get the need for speed and digest quantitative metrics like water. Another reason is just that giving people tools that work at speeds that approach
the speed of human thought can only make them more productive and happier (makes the human-computer connection more seamless).

We address the skill set
issue by exposing a search-based interface to the data. The search-based interface is much like Google: you type what you think and the search engine
returns some results that are likely to be useful to you (caveat: at this point, most of us have probably been using Google for so long that we have adjusted
our search styles to be more efficient against Google. Also, Google has steadily been experimenting with new ways to present knowledge. They've added
new preview boxes that pull in data from Wikipedia or Google Images into a convenient side bar fixture. They've also added instant search suggestions and
recommendations for related searches. Mini widgets for weather or translation also make the search experience more seamless. Who said that a list of blue
links with a robots.txt description was the most efficient way to get people answers to their questions?). The interface isn't *exactly* magic, because
it does require a lot of high-touch implementation from our awesome crew of architects and customer success managers and SREs and etc (that's the nature of
the enterprise software game; nothing to be surprised by here), but it does provide a clean, open interface with features like tabular data previewers,
lists of all the data sources and their associated column names, usage based ranking which primes the search suggestions. These features help new
users feel comfortable getting started with their company's data, be it P&L or system uptime or MixPanel click data. It's hard to explain the feeling of
being in front of a ThoughtSpot system in words. Please check out this [demo video](https://www.thoughtspot.com/product) to get the full experience.
We are all about empowering the end user, and I think after you watch the video you will appreciate how search lets people across the world get immediate
access to the data they need to do their jobs *right* and *well*.

The other amazing thing that
ThoughtSpot has done to improve the information retrieval experience is to
[abstract away joins](https://patents.google.com/patent/US20190303405A1/en?assignee=thoughtspot&oq=thoughtspot).
This is a really powerful feature of our backend query generation engine. Data admins only need to define joins once, when they are importing their DDL
and schemas into our system. Once those joins and their directions are loaded in (you can model the joins in a database schema as edges in a
directed graph), we use graph traversal to figure out the optimal join path for a given input query (e.g. "top 5 departments by profit 2018"). This engine
can handle multi-table joins, including joins across chasm and fan traps, and can detect join path ambiguities, which require human resolution. The power of
this system is immediately evident when you compare the processes built into a tool like Tableau. Tableau requires users to do additional modeling just to
[JOIN MULTIPLE TABLES WITHIN A *SINGLE* DATA SOURCE](https://www.reddit.com/r/tableau/comments/bhtb0n/heres_how_to_join_multiple_fact_tables_within_a/). We do
*all* of that messy work for you at search time. You just have to make sure the input schema is correct! One practical way to think about the implications of this
engine is: as long as the data is in our system, we'll get it back to you. What an amazing proposition!

Man, I could go on for a long time about other cool features, but let me also say that ThoughtSpot natively supports querying at any level of the data. You can
drill down into any column in a chart along any axis (Tableau requires manual creation of drill down paths). You can show the underlying data powering an
aggregated result at any time.

Before you say "you're exaggerating!", let me just say that we are only 2% done with our journey. Many of the features I've mentioned here are still in active
development because there's always accuracy and performance gains to be had on a complex system like this. There's also so many more things coming up in the pipeline
that you as an engineer, product manager, sales person, marketing person, data lover, or potential customer should be excited about. If any of the things that I've
discussed so far excite you, please don't hesitate to [email me](mailto:ipacifics@gmail.com?subject=Let's Talk ThoughtSpot) or message me on
[LinkedIn](http://linkedin.com/in/yangbianca/). I'd be happy to share more about my experience, answer any questions,
resolve any disbelief, and help you find a position at ThoughtSpot that will allow you to showcase your skills and become an even greater version of yourself.

<u>Culture</u>:<br>
The culture is honestly one of the most energizing I have been in. People are genuinely interested in each other's personal development
and in the company's progress. You have access to anyone in the company. Would you like to chat with our CTO about distributed data structures
or [machine learned indices](https://arxiv.org/abs/1712.01208)? Just walk over to his desk and chat. Would you like to learn about our marketing
strategy and what being in the [Gartner Magic Quadrant](https://www.thoughtspot.com/press-releases/thoughtspot-named-a-leader-in-the-gartner-2019-magic-quadrant-for-analytics-and-business-intelligence-platforms) means? Go ahead and Slack our director of marketing to schedule a time for
lunch. Want to be on a user study review panel? Slack the user study leader. Want to go on a customer meeting with one of our sales engineers?
Just ask.

You have no barriers to your advancement at this company except your own inhibitions. Let go of them and embrace the opportunity to learn from
our awesome team what it takes to build and sell enterprise-grade software and to manage the team behind that software.

<u>Interview Process</u>:<br>
You can expect 1 - 2 phone screens and 4 technical interviews during the onsite. One of your technical interviews will be a resume
deep dive. The other three interviews will go into algorithms, data structures, and coding proficiency.

If you interview for a new grad position, most of your on-site interviewers will likely be from the team that we think
is the best match for your previous experiences and thus presumed interests.

We are looking for people who are interested in refining the ability to craft software systems. We expect you to have good
coding and problem solving ability. Especially if you have database inclinations, we will expect you to have some basic systems
and OOP design abilities (understanding threads, unix, OS concepts, etc). We also look for good communication and attitude, but
the technical evaluation takes precedence.

<u>Projects</u>:<br>
You can get a sense for the trajectory the engineering and PM teams are on by looking at our
[release notes](https://docs.thoughtspot.com/6.0/release/notes.html).

Ask me anything about ThoughtSpot by [email](mailto:ipacifics@gmail.com?subject=Let's Talk ThoughtSpot).
