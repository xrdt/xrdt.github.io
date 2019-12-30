---
layout: posts
title: "Some Color on ThoughtSpot Engineering (Mostly Relevant for New Grads)"
---
*Author: Bianca Yang*<br>
*Email: <a href="mailto:ipacifics@gmail.com?subject=Hello from the XDRT Blog">ipacifics@gmail.com</a>*<br>

This is partly to document the current state of the system and to help candidates understand what they could be
getting into.

<u>The Five Engineering Teams</u>:
* Falcon (our in-house database and manages data loading interfaces)
* Sage (search engine. Responsible for tokenizing input and turning input into intermediate SQL-like query. Also responsible for surfacing
completions as user types into search bar)
* Callosum (application server that manages connections between Sage -> Falcon and Falcon -> Blink. Also translates the output from Sage into
the database query language Falcon understands)
* Blink (front-end)
* Orion (cluster management)

<u>Quality of Work and Quality of People</u>:
Choose who you surround yourself with carefully, because, like it or not, they will influence how you think, how you act, and who you
become. Choose to work in places that value craftsmanship and quality and (some level of) perfectionism. It will raise your bar to be around
people who produce at a high level.

It is hard to convince someone who has never interacted with our team or our codebase that we have excellent minds working on an amazing
piece of software. If you do come to do an onsite interview, I believe the quality of the team will shine through. If you look through our
codebase, you will realize that the foundational structures our core team of engineers who were responsible for building Bing, Google Borg
(which led to Kubernetes and Docker), massive infrastructure for delivering ads at Google and Amazon were extremely well engineered for
efficiency, extensibility, testability, and ease of use. This is undoubtedly a great place to learn the *craft* of software engineering and
will prepare you to build large scale, performant, and secure systems.

<u>Culture</u>:
The culture is honestly one of the most energizing I have been in. People are genuinely interested in each other's personal development
and in the company's progress. You have access to anyone in the company. Would you like to chat with our CTO about distributed data structures
or [machine learned indices](https://arxiv.org/abs/1712.01208)? Just walk over to his desk and chat. Would you like to learn about our marketing
strategy and what being in the [Gartner Magic Quadrant](https://www.thoughtspot.com/press-releases/thoughtspot-named-a-leader-in-the-gartner-2019-magic-quadrant-for-analytics-and-business-intelligence-platforms) means? Go ahead and Slack our director of marketing to schedule a time for
lunch. Want to be on a user study review panel? Slack the user study leader. Want to go on a customer meeting with one of our sales engineers?
Just ask.

You have no barriers to your advancement at this company except your own inhibitions. Let go of them and embrace the opportunity to learn from
our awesome team what it takes to build and sell enterprise-grade software and to manage the team behind that software.

<u>Interview Process</u>:
You can expect 1 - 2 phone screens and 4 technical interviews during the onsite. One of your technical interviews will be a resume
deep dive. The other three interviews will go into algorithms, data structures, and coding proficiency.

If you interview for a new grad position, most of your on-site interviewers will likely be from the team that we think
is the best match for your previous experiences and thus presumed interests.

We are looking for people who are interested in refining the ability to craft software systems. We expect you to have good
coding and problem solving ability. Especially if you have database inclinations, we will expect you to have some basic systems
and OOP design abilities (understanding threads, unix, OS concepts, etc). We also look for good communication and attitude, but
the technical evaluation takes precedence.

<u>Projects</u>:
You can get a sense for the trajectory the engineering and PM teams are on by looking at our
[release notes](https://docs.thoughtspot.com/6.0/release/notes.html).

Ask me anything about ThoughtSpot by [email](mailto:ipacifics@gmail.com).
