+++
title = "Announcing FLOSS/fund: $1M per year for free and open source projects"
date = 2024-10-15
authors = ["knadh"]
description = "Announcing $1 million per year in funding for Free and Open Source projects globally"
+++

TLDR; [Apply now](https://dir.floss.fund/submit)

----------------------

We are excited to announce the launch of a dedicated fund aimed at providing financial assistance to Free/Libre and Open Source Software (FOSS/FLOSS) projects globally, with an annual commitment of $1 million. I will use the FOSS acronym in this post hereafter.

This has been in the works for some time at Zerodha<sup>[[↗]](https://zerodha.com)</sup>, where we have been developing financial technology products and services built on an ever-growing FOSS stack. Without the high-quality FOSS projects that we have freely downloaded and used to build our organisation, products, and services, we would not exist as we do today—free as in both cost and freedom. A significant portion of our success and growth is owed to FOSS, encompassing everything from programming languages to operating systems, to databases, web servers, frontend frameworks, productivity tools, code editors, and absolutely everything. It goes without saying that this holds true for nearly every technology company founded in the last decade, whether it is publicly acknowledged or not.

And yet, funding and financial sustainability, the lack thereof really, has been an increasingly hot topic over the last many years. Well, at least since *cloud* companies began making massive profits directly repackaging FOSS projects built by hobbyists and communities. The rise of the "open core" model and the unfortunate license changes in many good open projects recently, are clear signs of this growing turmoil. Many potential solutions seem to be emerging and evoling—commercial services, Venture Capital (VC) funding, and programs like GitHub Sponsors<sup>[[↗]](https://github.com/sponsors)</sup>, Open Collective<sup>[[↗]](https://opencollective.com)</sup>, FUTO<sup>[[↗]](https://futo.org)</sup>, Polar<sup>[[↗]](https://polar.sh)</sup>, and *Buy me a coffee*<sup>[[↗]](https://buymeacoffee.com)</sup>, amongst others. That said, Python libraries raising massive amounts of VC funding in quick time does not look like a healthy trend.

Why are we here, though? The fundamental tenets of FOSS, the spirit of hacking, liberty, and reciprocity, while they have worked beautifully with code, have translated poorly into the highly commercial *BigTech* era. So far, it has been nearly impossible to quantify and structure ideas of goodwill and reciprocity into financial sustenance for FOSS projects. I recall the log4j incident from a couple of years ago which unleashed a spate of philosophical debates around  FOSS, in which I also participated<sup>[[↗]](https://nadh.in/blog/open-source-is-not-broken/)</sup>, rather ideologically.

For us, FLOSS/fund is about hacker goodwill, reciprocity, and common sense business strategy. We invite you to [apply for funding](https://dir.floss.fund/submit). If you would like to understand the motivations behind this, a bit of storytelling lies ahead.

## Prelude

The very first thing I did when we started Zerodha Tech more than a decade ago was to install Python and start scripting and automating time-consuming, mundane organisational tasks. Then came Postgres for building a small data warehouse, followed by PHP and WordPress for managing our website. From there, as we slowly grew the organisation, our technology stack expanded one piece of FOSS at a time, eventually leading to us becoming the largest stock broker in India several years later. Personally, my mental markup as a software developer and hacker is rooted in the simple act of copy-pasting open source code from the internet to hack, tinker, learn, and solve problems. An alternate vision is very difficult for me to comprehend, and a non-FOSS path to building technology, let alone an organisation, has never seemed logical.

<!-- The funny thing is, Zerodha is a heavily regulated financial services firm working with regulated, licensed, and proprietary services and data from Indian market institutions. Every aspect of the software and services (web and mobile investment apps for instance) a broker can offer in India is regulated—everything from font sizes to the dimensions of certain popups to being manadated to offer specific features to having to display the version string on the UI in a certain format (!). Many software changes have to go through certification and approval process. Exchange connections and connectors required to facilitate transactions, financial risk models mandatemandatedd by regulations, are all licensed and proprietary and only available at physical leased line termination points with regulatory approvals. In India, it is legal only for a stock broker to offer investment and trading apps. Offering HTTP API connectivity to end users may soon become "illegal" (!) Investment platforms in India, thus, can only operate as "SaaS" applications under strict conditions. And yet, behind the scenes, our stack, and certainly most other players' in the industry, are built on FOSS. !-->

At Zerodha, over the years, we have contributed upstream to many projects that we use, as well as spun off and released several small and large FOSS projects<sup>[[↗]](https://zerodha.tech)</sup> from our work. In 2019, we made a sizeable investment in ERPNext<sup>[[↗]](https://erpnext.com)</sup>, a FOSS ERP that we had begun using extensively. In 2020, we co-founded the FOSS United Foundation<sup>[[↗]](https://fossunited.org)</sup>, which works on developing the FOSS ecosystem in India, and backed the creation of TinkerSpace<sup>[[↗]](https://www.tinkerhub.org/tinkerspace)</sup>, a physical hackerspace and community center that hosts FOSS tinkering for young people. In 2023, we were a founding member of OASIS (Open-Source Alliance for Social Innovation and Sustainability)<sup>[[↗]](https://oasishq.org)</sup>, which focuses on FOSS capacity building and adoption in social sector non-profit organisations. Many of us from our team also volunteer at non-profits, helping drive meaningful FOSS adoption in the development sector, where even basic technological requirements are woefully unmet. We fund many of these initiatives with long-term commitments.

In addition, we have given out many sizeable grants to FOSS projects and organisations in India. While funding projects outside India involves significant paperwork and operational overhead, we have reached out to several small and large projects that we use at work and have managed to pay them. This highly ad hoc approach is something that has increasingly bugged me though.

While it is good to provide financial support to FOSS-aligned activities, most importantly, money ought to go directly to the source—invaluable FOSS projects. We have managed to build a commercially successful business on top of FOSS that we have freely, in both cost and freedom, adopted from all over the world. Therefore, "ad hoc" and "reaching out" simply do not suffice—we have to shut up or put up.

## Thus, structure.

And that is how the idea of a structured, dedicated fund for FOSS projects globally, was born. We spent several months speaking to various banks, payment processors, and lawyers to finally arrive at a reasonably streamlined process. The fund will:

- Have a small, dedicated team to operate it properly in a non-adhoc manner, functioning like an OSPO (Open Source Program Office) but focused on funding projects—an OSFO (Open Source Funding Office), perhaps?
- Put money where the mouth is—a minimum of $10,000 and up to $100,000 for a single recipient, totaling $1 million per year, which we will increase once we understand the dynamics of running the fund.
- Source applications globally, relying on incoming applications through for discovering projects in need of support rather than the limited visibility we have as a small team.
- Form an interim internal investment committee to make discretionary selections. Once potential edge cases and any gotchas in running the program are handled, we will attempt to establish a public selection committee from the FOSS ecosystem with a community voting process for applications.

## More structure: funding.json
Expanding a bit on "ad hoc" and "reaching out" I mentioned earlier, the  majority of our experience paying projects has transpired like this:

On a random day, we realise that a certain FOSS project has become very useful to us. After a bit of online searching, we find the developer's email address. We write to the developer, thanking them for their work, explaining how useful we find it, and expressing our interest in financially supporting it. They respond, thanking us but stating that they have not thought of any specific numbers. After a bit of friendly back and forth, we suggest an arbitrary amount, followed by more discussion about logistics and paperwork. This process of arriving at numbers over personal e-mails is akward for both parties. It addition, it typically takes weeks, requiring time, commitment, and bandwidth from both the developer and the donor to complete a single transaction. Models like Open Collective and GitHub Sponsors address this to some extent, but there is no open, decentralized mechanism for discovering projects in need of financial assistance nor gaining insights into their specific needs.

Any attempt on funding FOSS projects generally warrants clarity on several questions.

- Does the project under consideration need financial assistance?
- Or perhaps it is not just one particular project, but a developer or a group of developers who maintain several projects that need assistance.
- What kind and quantum of financial assistance are needed, and for what activities? Is there a structured support plan that the developers offer?
- Has the project received any funding in the past? Is it in dire need of support, or is it doing reasonably well?
- What payment methods are accepted? Is there a payment link or address that can be used without manual contact, or is something like a bank wire that is required?
- Once there is enough context, and a conversation is warranted, how does one reach out to the right person who address financial or logistical queries?
- That's about one project. But what about a particular category of projects? Maybe it is an emerging or critical area, and it would make sense to support multiple projects there. How does one discover them?

What if the answers to such questions could be structured in a machine readable format, which could be crawled, indexed, catalogued, and made discoverable—similar to a `robots.txt` or `package.json` or `sitemap.xml`, but for funding. In the process, eliminating a lot of awkwardness and apprehension that would be otherwise transpire over back-and-forth personal e-mails discussing financial matters.

How about a standardised <code>funding.json</code> manifest file that can be added to project repositories and websites signalling their financial needs? Something like this:

```python
{{ read_file(path="static/static/funding.example.json") }}
```

To initiate and give this experiment a serious shot, FLOSS/fund will accept funding requests from projects through a publicly accessible <code>funding.json</code> file hosted on their respositories or websites. This file is not meant to convey everything there is to know—an impossible task—but to solicit interest and communicate enough to ensure discoverability which would not be possible otherwise. Refer to the [funding.json docs](/funding-manifest) to know more.

Applications that come through to the FLOSS/fund will be indexed and published on the [dir.floss.fund](https://dir.floss.fund) directory / portal, making them publicly discoverable by anyone interested in supporting projects. This is going to be an interesting experiment. Fingers crossed!

## Motivations
What are the motivations behind the fund? On a personal level, it is common sense, goodwill, and reciprocity—the spirit of FOSS. From a for-profit enterprise perspective, however, terms like "goodwill" and "reciprocity" are notoriously problematic, and most likely fundamentally incompatible with their very nature. But, that is a separate philosophical debate altogether.

Setting philosophies aside, it makes perfect logical sense for a business that relies on FOSS to support it, directly or indirectly, when they freely tap into a global ecosystem of unlimited FOSS innovation—free in both cost and freedom. How many technology companies today could even exist without the massive amounts of FOSS they use? Ensuring that this ecosystem thrives, without inadvertently turning parts of it into a classic tragedy of the commons, everything aside, is good, logical business strategy. At the very least, a profitable business should allocate a tiny fraction of its profits to support the projects it is directly reliant on. When many startups have advertising and marketing budgets that often put public spending to shame, one would be hard-pressed to find a reason not to give a bit of money  to the projects they depend on for their very existence.


Thus, FLOSS/fund's motivations are to:

- Exercise our goodwill and reciprocity on a personal level as FOSS hackers.
- Exercise our organisational business sense and strategy to help the FOSS ecosystem thrive, without which our business cannot exist.
- Encourage and apply a bit of peer-pressure on other businesses to setup structured financial support programmes for FOSS.
- Contribute to existing FOSS funding models and to the sustainability conversations and debates.
- As a bonus: Explore whether the `funding.json` manifest experiment can bring discoverability to the financial needs of FOSS projects on a large scale.

Let us see how this goes.

<div style="text-align:center"><a href="https://dir.floss.fund/submit" class="button">Apply now</a></div>
