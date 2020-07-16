---
layout: posts
title: "Stepping into the Field: Enterprise Sales Trip Dec 2019"
---
*Author: Bianca Yang*<br>
*Email: <a href="mailto:ipacifics@gmail.com?subject=Hello from the XDRT Blog">ipacifics@gmail.com</a>*<br>

I went on a sales trip to a customer that just signed an expansion deal with us on Dec 9 - Dec 11. I'd been
wanting to go visit a customer for a while at that point, so I could get grounded in the all important,
oft-talked about but infrequently sought for insight into "user experience".

Our team spent 1.5 days with the customer, teasing out the exact use cases and teams that our product
could serve and the data sources we could pull into our application. I was not an active participant
in any of the meetings. The sales engineer, account executive, customer success manager, architect, and
internal liaisons / champions did the hard work of understanding what business questions people are trying
to get answered, whether there is pain in getting those questions answered, and how we could elevate the
affected teams by alleviating the pain of getting insights.

Selling is really bloody hard, even when you don't have to sell through a whole day of 2-hr meetings where
people appear to be so blocked by systemic inefficiencies in their data access and analysis tools that
they can't see how moving their data into our tool help them switch from fire-fighting operational
snafus to devising strategic initiatives for their org 2.0. When you work in Silicon Valley, you are surrounded
by people who have the most lofty goals and intentions when it comes to leveraging bits to get to an elevated
state of being. The bubble is real, so it's good to get grounded in the reality of the grimy, manual,
fragmented processes that govern the daily operations of your customers so you can
[BUILD](https://web.archive.org/web/20140208033540/http://betashop.com/post/32913573235/90-things-ive-learned-from-founding-4-technology)
[THINGS](https://blog.samaltman.com/startup-advice) [THAT](http://www.defmacro.org/2013/07/23/startup-lessons.html)
[MATTER](https://web.archive.org/web/20130919195047/http://betashop.com/post/1417413108/57-things-ive-learned-founding-3-tech-companies).

What I heard in hour after hour of meetings was that most of the company's BI problems are DATA problems
([The three most common BI problems: slow query performance, lack of interest from business users[[1]](#1d)<a name="1u"></a>, and poor
data quality.](https://bi-survey.com/bi-avoiding-problems)): (The below are paraphrases.)
* "The tool is only as good as the data we feed into it."
* "__Most of time my team's output is Excel data dumps.__"
* "I'm laughing because you made it sound like the suppliers are just giving us data. We have to grab the
data from them."
* "__We have the data from factory to port and we have the data at stores / warehouses__. What we don't have is
data that lets us link the shipments sitting at port to our stores / warehouses, which results in allocation
and planning problems."
* "I want to know what is going on in the warehouse, at the pick and pack level, but we simply don't have access to
that data."
* "We all want to answer the same business question: why isn't my order where it is supposed to be?"
* "We don't have good historical data on freight spend, so our forecasting and negotiations are based on simple,
linear Excel models."

ThoughtSpot's system can't solve data access issues, but we can certainly help with
people getting access to the subset of supply chain data they need to do their jobs. I bolded the few statements above that
indicate that people have data but are stuck on getting access to the relevant subset. Those situations were the basis for the
the use cases that we presented to the data team on the following half day. This is where things started to get
interesting. The data team made it seem like they had built a centralized table with practically everything any of the supply chain teams
would want to know about the health of the shipments. My team was really confused about where the pain was...especially since this
centralized table was only 15mil rows (no problem for TS's system, which can handle billions of rows). Apparently every team is accessing the same
dataset (of only 15mil rows). There was some unresolved uncertainty here between what the data team and the analysts / business users
were telling us, which I expect the sales team will refine and resolve through the implementation process.

Over the course of these two days, I really began to understand what it means to build sales relationships. All of these meetings
happened because we managed to find a great champion at the company from our previous engagement with a different org.
Our champion has an excellent understanding of the landscape of data-related pains within the company and an real knack
for talking to senior leadership, both things we needed to kick start our penetration into the account.

This was where I came to the conclusion (or do you want to flatter me and say "insight") that willpower is the fuel
for making things happen. Every meeting, every interaction we had with the our (potential) customer had to break through
the wall of lack of interest. Even if your first contact has a lot of passion for the product and wants to move forward, it's
a nontrivial task to maintain the momentum and interest and build a road full of meetings that take you through the finish line of
a successful deployment.

A few days earlier, I had the thought that curiosity was the spark for getting people to make things happen. Now
with willpower to sustain the curiosity-driven inspiration, we have a formula for getting things done. But here
comes the inevitable caveat: how do you know that what you're doing matters? Hem and haw all you want, but
there's already pretty good answers on the market about product market fit.

[[1]](#1u)<a name="1d"></a> We didn't encounter any cases where there was lack of interest from business users,
but we did have an unfruitful meeting with just _analysts_. These analysts' day to day jobs were one level removed from the
business user. These analysts are largely responsible for providing technical support to analysts that directly interface with the
business users, so they couldn't see value in adding our product to their team. While analysts are an important part of the
value chain, our proposition of delivering an unparalled self-serve, search-based analytics experience is most compelling
to business users. Business users are the ones who are suffering from lack of data and therefore lack of ability to make
data-driven (informed) decisions about how to deliver upon imperatives from their leadership to innovate upon the current state of the business.
