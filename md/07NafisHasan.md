---
Pr-id: MoneyLab
P-id: INC Reader
A-id: 10
Type: article
Book-type: anthology
Anthology item: article
Item-id: unique no.
Article-title: title of the article
Article-status: accepted
Author: name(s) of author(s)
Author-email:   corresponding address
Author-bio:  about the author
Abstract:   short description of the article (100 words)
Keywords:   50 keywords for search and indexing
Rights: CC BY-NC 4.0
...


# ‘SLOW VIOLENCE’ AND VACANT CITIZENSHIP: THE EXCESSES OF INDIA’S DIGITAL GOVERNANCE

### NAFIS AZIZ HASAN

## Introductory Note

This essay emerged from a recent encounter with the tumultuous world of
technology producers working to transition the Indian state into the
realm of the digital. Expecting to be schooled in the technical
apparatus of the transition, I interviewed, in 2018 and 2019, multiple
engineers and technical experts in various roles, capacities, and
inclinations. Yet, instead of a grandiose telling of the potential
transformation to governance and life, these conversations revealed an
anxiety about data, about the imminent dangers of the transition, and
the sheer unpreparedness to tackle the still largely unknown but
creeping threats that data posed. Categorized as hacks, leaks, malware,
or SQL injections, these experts nervously warned that the gov.in was
under siege from within and without. Far from the total and uncritical
adoption of digital forms, these experts advised a cautious use of
technological products, prescribing ways to wipe out one’s digital
trail. Indeed, many made elaborate arrangements to leave no trail of
their personal information on the computer systems they worked on.

In these conversations, the source of this danger was somewhat
unspecified and, when named, not consistent. Sometimes it was Israeli
hackers exploiting their weak information technology (IT) laws,
sharpening their jacking skills on poorly protected Indian systems;
other times it was simply bad design. Yet, the crisis was palpable and
the discourse of the imminent danger was reaching scalar proportions.
State governments were being forced to discuss it in their Question Hour
and senior officials were laying out a counterstrategy in the form of
hiring an army of ethical hackers to preempt and foil potential attacks.
Media reports and other writing were bolstering these fears by
quantifying casualties: ‘Over 22k Indian Websites, 114 Govt Portals
Hacked between Apr 2017-Jan 2018’, read one newspaper report.[^07NafisHasan_1]

Standing for a moment outside this threatening
present, one begins to see that the dangers being alluded to are in
response to an original expectation from the juggernaut of digitization.
This was an expectation of mobility, where information firmly lodged in
government documents turns into mobile data, available as a knowledge
input in the many decisions that make government. The deviance of data
from this linear path toward something else is a phenomenon that comes
after decades of the digitization machine at work, possibly a reason for
the grave reactions toward it. There is a robust, if brief, history of
the datafication of government, which is not often recalled but is a
reference point of the current predicament. Historically speaking, what
we see now is a situation I term excess. Excess or the excesses of digitization become a vantage point to
illuminate the historical conditions and trajectory of digitization as a
changing technopolitical assemblage of people, ideas, and technologies
and their effects beyond expected outcomes. Other people interested in
this history have asked and convincingly pointed out to the many
political choices that have led to the present. In other words, we have
some scholarly excavations of *why* digitization is in the state it is
in. Somewhat uniquely, this essay asks not why
but *how* we reached here. Also uniquely, the story of this how is
revealed through a technological object: database management systems as
a conglomeration of code and algorithms that came to define and direct
the mobility of data, the dividing line between analogue and digital.

Relating the story of the present through a technical object doesn’t
mean getting lost in the intricate technical details of management
systems, fascinating as that might be. This essay aims to strike a
balance. On the one hand, it is eager to point out remarkable shifts in
technical configurations that initiated an altogether new direction and
scale of the digital. The one big moment this essay highlights is the
revolutionary innovation in coding data through algebraic relations that
allowed manipulating it from a distance. To some, this may seem as a
primitive technological past of the 80s and 90s. Yet, the reason I focus
on revolutionary design of relational databases is because not much has
changed in use by governments. There are very few examples of the use of
non-relational databases in government (India’s biometric project
Aadhaar is one example) and it seems like a procurement problem with
governments all over the world, not just in India.[^07NafisHasan_2] On the other
hand, the essay works hard to illuminate the social and political
dimensions of these purportedly technical changes. How does an algebraic
relation used to arrange data change our relations with each other and
with institutions? Such a hyphenated inquiry encounters political
concepts: neoliberal politics, rights, citizenship, access, and takes
them head on. Unending servers of data at the 400-odd National
Informatics Centres (NICs) strewn across India, leaching in and out of
myriad computer systems, unsettle notions of neoliberalism exclusively
built on a separation between state and market. Excesses in the form of
hacks, leaks, and errors in data produce new obligations on individuals
needing this data to exercise their basic rights. Excess offers a
vantage point from where to view citizenship practiced and experienced
as a tryst with broken data.

This essay is not simply about the social life of databasing techniques,
even though a significant amount of space is dedicated to telling that
story. It is, at its very core, the thick description of a total social
fact that pervades all forms of datafication. Social facts are things
external to individuals and specific situations, but have significant
effects on material life. Databasing techniques are similarly concealed,
but central to the movement of data, so as to not be seen or recognized
as critical components to the story of digitization. Yet, as this essay
reveals, they constitute the basis for the materiality of information.
They give data a form and interpretive possibilities. They also, as this
essay shows, make data potentially dangerous, going beyond the
conditions of its arrangement.

**I**

## REMAKING GOVERNMENT IN THE REALM OF THE DIGITAL

## The techno-politics of neoliberalism

In 1993, Infosys recorded revenue of \$5 million.[^07NafisHasan_3] One year later,
that had jumped to \$9 million on the back of Finacle – a banking system
that centralized customer data to a back-end database system, while
allowing a proliferation of service at myriad front ends: at the branch,
in the home, or online. 
In a short period of time, Finacle went from 10 banks to 100,
and then rocketed to 1,000 banks across 150 countries.[^07NafisHasan_4] A year later,
in 1994, the automobile company Maruti introduced an Oracle database to
keep track of a million moving parts in its Gurgaon manufacturing
assembly, significantly reducing production time.[^07NafisHasan_5] Likewise, bourses
in the mid-90s like the National Stock Exchange, the Delhi Stock
Exchange, and the Pune Stock Exchange introduced a dual database and
screen-based order-and-quote trading system that made multisited access
possible.[^07NafisHasan_6]

What explains this momentous transformation in the sheer extent of data
transactions in these diverse domains? Service, during this time, got a
new name. From hugely deficit, long-waiting lines of poor service
experience, India began to see quicker, multiple points of service
access. Underlying this emergence of what has been called ‘modern
services’ was a revolution in data storage design that crucially allowed
access to data from locations other than where it was physically
located. 

In 1973, Edgar Codd, a computer engineer at IBM in San Jose,
California, invented a new ‘relational’ way of storing data that would
fundamentally transform how data was being accessed across the world.
Called the relational database management system or RDBMS, he developed
a system of symbols borrowed from algebra to define multiple
relationships between dimensions of data. The format in which the data
now came to be stored was the table, as opposed to a tree-like or
hierarchical structure. This did two things to revolutionize access. It
brought about ‘data independence’, that is, a separation of the
application querying data from the structure of data storage itself, and
it allowed access to data without the need for an underlying knowledge
of where the data is stored on a disk.

This meant that one did not have to be a trained computer engineer to
query a database. People with less technical knowledge (and possibly
more business knowledge) could also formulate queries. With rapid
increases in information communication through networks, widespread
querying became possible from locations away from the data source. This
gave businesses in the United States a phenomenal opportunity to analyze
information from multiple locations and make decisions about stocking,
pulling out, and pricing practically in real time. Between 1973, when
Codd developed this model, and the early 80s, the market for RDBMS grew
to, by one estimate, about \$130 million.[^07NafisHasan_7]

RDBMS has sometimes been named, retrospectively, as a ‘disruptive’
technology. Materially, databases have been over the past 40 years
surrounded, supplemented, and displaced by other forms of record
keeping. Conceptually, digitization, or the process of turning analogue
data into digital forms, is more often than not talked about, thought,
and imagined as things that are encoded and represented in databases.
The computer scientist, Paul Dourish,[^07NafisHasan_8] echoing an entanglement
between prior technologies like writing and the practices they engender,
says that ‘when the database is a tool for encoding aspects of the
world, the world increasingly seems to us as a collection of
opportunities for databasing’. RDBMS, and its ‘disruption’, was not
simply a technical infrastructure, but rather an *assemblage of
technical choices and political outcomes*. Studying it as a *cultural*
phenomenon (as I do in this essay) has thus involved identifying it
within a triad of database functions, infrastructural arrangements, and
informational practice.

When this disruption reached India in the late 80s and early 90s, it was
initially brought to life by IBM on the back of Rajiv Gandhi’s New
Computer Policy that, after stonewalling foreign investments for a
decade, now permitted their entry into technology production. As it did
so, India found itself on the brink of another disruption. In 1991, when
Prime Minister P.V. Narasimha Rao, after years of debate, finally
dropped the axe on the liberalization policy, RDBMS was just about
picking up. Indeed, this essay makes the (provocative) argument that the
trajectory of post-liberalization would soon be fundamentally entwined
with the trajectory of RDBMS as the infrastructure that came to define
neoliberalism began to coalesce into its backbone, namely India’s
growing service sector. Such an argument departs from the conventional
history of technology development in India, mostly presented (for
example, in a recent book by Mohan Sukumar)[^07NafisHasan_9] as the mute result of
dramatic political choices. Likewise, liberalization has itself been
conventionally viewed through a political economic lens of a withering
state and emerging markets, and less often in its cultural impact on
personhood.

While emphasizing what I see as the tectonic
effects of a single technology, I do not elide the political; indeed, I
hope to provide something of a techno-political account of
post-liberalization in India: the ways in which political actions are
embedded within technical forms and, conversely, technical objects shape
political questions. Techno-politics, in its contemporary usage, often
reveals engineering or infrastructure projects as vehicles for political
goals and forms of power. It thus foregrounds political abstractions in
a very material way. As a form of postcolonial computing, RDBMS can be
seen as an assemblage of technologies, techniques, and desires
undergirding shifts in neoliberal governmentality, enabled by
significant interventions in multiple definitions of personhood that, in
turn, define both privacy and surveillance as well as widen the domains
of economic rights as these extend to the identification and targeting
of beneficiaries. The *forms* of data that RDBMS helped produce across
domains of life, including health, land, labor, and leisure, as well as
the *channels* of circulation it opened up – from home to kiosk to data
center and back – created a *radically new experience of citizenship*.
The changes in the early 90s that many have seen as nothing less than a
social revolution with significant legal, economic, and constitutional
consequences were, I argue, undergirded by databasing technologies.

Let us consider some of the ways in which the entry of RDBMS helps
account for the momentous changes that occurred in the 90s. One view on
neoliberalism sees it as taking place autonomously, in what Thomas
Friedman names ‘golden enclaves’ existing outside state
institutions.[^07NafisHasan_10] A look at the ‘national’
career of technologies suggests otherwise – the founding of the call
center industry in India that peaked in the late 90s, for example.

At its core, call centers allowed a translocation of services, produced
in one (geographic, territorial, sovereign) region and consumed in
another. What, we may ask, were the technologies that drove this? A lot
of focus has been on the internet and networks in general, but young men
and women in Bangalore, Gurgaon, and Mumbai were also accessing data
that was stored thousands of miles away. Some were, inevitably, stealing
that data and selling it to other companies – such as the famous case of
an HSBC employee stealing bank information and money in 2006[^07NafisHasan_11] – but
most of them were simply accessing personal, sensitive, financial data
of their British or American customers through application interfaces
that connected them to databases in those countries. Without several of
the features of RDBMS, none of this would be possible.

Crucial here is also the role of service providers contracted to run
call centers, build and run technology to access their client data, and
offer services. The costing models, the lynchpin of the business of
offshoring services, made sense only when Indian companies built their
own technology and then charged their customers on a pay-per-use model.
Companies like Genpact and Mphasis were now buying proprietary RDBMS
from companies like Oracle and Microsoft to run their centers. Without
that, it would have been prohibitively expensive to import RDBMS and to
make the call center business profitable for firms abroad.

The point of this example is to show that
tracing the career of technologies of neoliberalism such as RDBMS can
*reconceptualize neoliberalism itself*, taking it away from Friedman’s
golden enclaves and into entangled governmental policies (allowing the
purchase of offshore database management systems in this case). It gives
us another, *opposite*, way to think about the history of the present.
Calls among neoliberalism’s leading promoters, such as the World Bank,
have often been framed around advice like the trite ‘less government
more governance’ line. But growing scholarship on both liberalism and
neoliberalism has shown that lesser or leaner government does not
necessarily translate into either less regulation or weaker states.[^07NafisHasan_12]
Indeed, it proliferates the sites for regulation and domination by
creating autonomous entities of government that are not part of the
formal state apparatus but are instead guided by an enterprise logic.
This is indeed the *techne* of neoliberalism, in which states ends up
allying themselves with a range of other groups and forces, and seek to
set up ‘multiple chains of enrolment’[^07NafisHasan_13] that mask the state’s
persistent presence through ‘government-at-a-distance’ approaches to
governance.

An oft-cited example of neoliberal governmentality, government-organized
non-governmental organizations (more popularly referred to by the sonic
acronym GoNGOs) too have been innate to the transformations of
government, and mediate governance into the several new distributive
possibilities that technological infrastructures increasingly allow.

RDBMS apparently illuminates this better than these new institutions can
do on their own. To take one example,[^07NafisHasan_14] in 2012, Mother NGO or MNGO,
set up by Chief Minister Sheila Dixit’s government in Delhi, conducted a
massive GIS survey of Delhi’s homeless population to map their
geographical coordinates and to create locative identities in the
absence of residential ones. Inevitably, the data generated by the
handheld GIS tracking devices that its surveyors used night after night
(nighttime location being a credible way, the surveyors fathomed, to
determine what they called ‘most visited location’) was stored on an
RDBMS. Such collection and storage thus allowed access to multiple
interested actors, including contracted surveyors, representatives of
MNGO, organizations working for and with the homeless in Delhi,
bureaucrats of the Delhi Urban Shelter Improvement Board, and the chief
minister’s office in the Delhi secretariat. Every one of these actors
could, via authenticating logins and interfaces, access locative IDs in
real time. This allowed a previously unfathomable level of control and
realignment of all of these agencies, and it also enabled a previously
unimaginable partnership between state and non-state actors that
challenged most received notions of either lesser government or more
governance.

‘Participation’, another keyword freely doled out as a neoliberal
expectation, also centrally features in projects that are on their face
foundationally located in welfare, such as the Mahatma Gandhi National
Rural Employment Guarantee Act, 2005 (MNNREGA), an Indian labor law and
social security measure, often presented as an antidote to
neoliberalism. MGNREGA’s entire logic of social auditing, a
much-celebrated aspect of its accountability mechanisms, was enabled
mainly by the ability of government officials and other multiple
beneficiaries to query an RDBMS database (for example, nodal agencies
both at district and central levels supervising the status of work,
payment, fund utilization and fund requirement). This data helps
government and citizens alike to in turn generate reports through which
both participation and accountability are ensured.

## Digital Governance as a Stratigraphic System

My aim is not to pick a random set of government endeavors and show the
value of RDBMS in them. My own examples, of call centers (a symbol of
India decidedly on the route to becoming a service economy) and MGNREGA
(as a prime example of welfare, at once a state-directed identification
for future dole and a means of enabling participatory governance) are
mainly to outline the latter career of two concepts – service and
welfare – that have been foundationally connected to the grand narrative
of India’s tryst, and eventual failure, with an industrial economy. Atul
Kohli’s argument about liberalizing reforms as neither helping nor
hurting India’s industrial growth[^07NafisHasan_15] is telling because it opens up a
space to think about the *copresence of welfare with a neoliberal
service economy*, despite the two being organized around different
logics. That RDBMS undergirds elements of *both* welfare and service
points to its centrality in shaping our populational experience as a
whole.

What I want to take on here, as a specific object of focus, is the
career of data and its storage within the story of the digitization of
administrative government in India. This is a site where both the
potential and the risk of RDBMS is at its most apparent. If RDBMS is the
concealed infrastructure of big data, there is another concealment at
play here: the vulnerabilities in data produced as a result of changes
to its storage design. The career of RDBMS in government shows us that
the modularity in the arrangement of data and better reach and access
sits side by side with the risks this arrangement of data poses. When
data was locked up on a computer – as it was in the earlier DBMS system
– it had remained secure. Any threat of manipulation had in part been
averted by the need to understand the basic structure of the data,
something that was no longer necessary with RDBMS.

Nowhere were the perils more acutely felt than in government itself.
Although the Indian state has been on the RDBMS wagon since the 90s, its
bureaucrats and their consultants have only recently ratcheted up the
conversation on data security. Although I recount older concerns with
data security later in this essay, and while I show that security was
thought about as early as the 80s, it appears that these did not curtail
the movement of data that RDBMS brought forth. The trade-off (between
data proliferation and security) is most evident in the digitization of
the apparatus of governance itself. It also raises basic questions
around how the proliferation of governmental data might be viewed within
the present-day excesses of big data. Was there a *weakening* of the
formidable forms of knowledge and control governments once possessed,
and thus a phenomenological crisis in the state as RDBMS disperses data
across locations and people?

This is a story that unfolds in a more or less stratigraphic
manner.[^07NafisHasan_16] The paper files of colonial-style bureaucracy had a system
– which database engineers hired by the Planning Commission in the late
70s and 80s abstracted and on top of which they built databases to serve
the needs of their massive planning exercises. When other innovations,
primarily RDBMS (but also Graphical User Interfaces GUIs and other forms
of networked databases), were in turn built on top of *that*, it changed
the organization itself and with it the flow of fast-digitizing
administrative data. A new set of relations now emerged in the
bureaucratic workplace, alongside an accretion of its functions and
processes, each changing at different speeds.

What we now saw was significant: a slow descent into chaos, instantiated
by spectacular leaks and hacks, mundane system breakdowns, errors and
loss of data, all of which reveal diverse layers of techno-politics
congealed beneath the benevolent-sounding term ‘electronic governance’.
Viewing the digitization of government in archaeological fashion, as a
series of layers, offers a history of the present. Although the
researcher’s access to details of any single layer remains always
incomplete, a through-line emerges *across* the layers, centered on the
*choice* and *availability* of data management infrastructure with their
accompanying political possibilities. Let me try to provide an outline
of each of these layers, which map onto the sections below.

As far back as in the early 70s, India's Planning Commission – dogged by
its recent history of ‘failed’ plans and frustrated by the poor quality
of information available to it from various sectors of the economy – had
sought ‘data improvement’ by constituting various committees. Since much
of this information pertained to numbers, and since number-crunching
organizations like the Indian Statistical Institute were already using
computers and automatic calculators, the Commission decided early on
to build computerized information systems. Yet the organizational forms
of bureaucracy within which this information lay was notoriously opaque,
with complex rules and minute levels of writing and inscriptions. This
information was embedded in writing files and records with intimate
channels of circulation and comprehension. The Commission soon realized
that, before computerizing information, they had to first help
bureaucrats in myriad ministries identify and digitize
information most relevant to planning.

As I browse through the noting, comments, rebuttals, and replies that
constitute the paperwork of these debates, now archived in another
bureaucracy (the National Archives of India), a growing turf battle is
discernible between scientists and bureaucrats. At the heart of these
debates is the question of control over information. Thus, when budding
Commission-supported computer scientists began considering, in the 70s,
how to develop a digital information system that would aid the Indian
bureaucracy in its production of knowledge about the world, as well as
how to make that information available to other bureaucracies away from
sites of action, they ran into two specific problems. First, *what*
information from specific bureaucracies should be digitized and
mobilized for action and *who* should decide this? Second, *how* should
bureaucracies share this information, through what means, how much, and
how often?

Attempts at digitizing (and subsequently computerizing) information on
which public bureaucracies depended for their existence set loose a
fundamental transformation in the nature of the information itself. In
hindsight, the crisis was initially one of boundaries. If information
production had so far worked through opaque rules and rituals of
writing, all of which demarcated bureaucracy from the rest of society,
how would the relationship of bureaucracy and society change when
information once lodged in office registers now became untethered and
mobile?

In the initial years of digitization, this
relationship did not change very much. Early attempts at dislodging data
concealed in dusty registers of district offices were, as I describe
below, thwarted by available infrastructure. While these attempts aimed
to make information move so that some center (either at state or
national level) could see this information as data, movement began to be
constrained by an overbearing fidelity to the organizational design of
bureaucracy, to its hierarchies and rules, as well as to the
computational design of information systems. In contrast, 30 odd years
later, the mobility of information as data, in the era of let’s say
Aadhaar, not only clogs the information highway, it storms into the
lanes, cracks, and crevices of daily life.

There is no single metric to determine the extent to which government
work has been digitized. But a range of examples exist that point to a
huge transition into the digital sphere. A technical director from
India’s National Informatics Center (NIC), which has spearheaded this
transition since the 70s, told me that NIC servers receive over
two million emails per day addressed to government employees.[^07NafisHasan_17] He
said this makes @NIC.in the largest email service in the world. In 2016,
the business magazine *The Ken* carried a long piece on
the ‘appification of the Indian *sarkar*’ (appification of the
Indian government), pointing out that the Centre for Development of
Advanced Computing or C-DAC was ‘churning out five or six apps every
month. Read that again: five or six new apps every month’.[^07NafisHasan_18] To point
out how much data that must be producing, the writer says: ‘It’s
happening at a scale so massive that there really is no comparison. Just
for perspective, the United States of America has a total of 218 apps in
its directory’.[^07NafisHasan_19] A land records digitization index, published by the
National Council for Applied Economic Research (NCAER) in February 2020,
shows that, barring four states, all other states in India have some
form of digital land records.[^07NafisHasan_20] 

Trying to excavate a chronology of digitization through reading
technological infrastructures shows how RDBMS enabled a foundational
national policy on the electronification of governance – the National
e-Governance Plan (NeGP), a set of projects that includes the
controversial Aadhaar project, to electronically provide governance at
different scales.[^07NafisHasan_21] Much has been said about its conception of
governance, about the financial investments it has attracted, and the
kind of relations between people and states this has engendered. Very
little, however, has been said (at least among people studying it as
policy) about its technological structure, which at its very core
instantiates a first, and eventually lasting, example of RDBMS in action
within the domain of digital governance.

The NeGP structure is outlined in more detail later in this essay. In
brief, however, it is made up of a core network of State Data Centres
(or SDCs) – physical locations that contain the databases along with
applications for storage, retrieval and manipulation of data, and
maintaining cyber security – connected with intranets. SDCs further
connected, through State Wide Area Networks (SWANs), to Common Service
Centres (CSCs) that delivered services to multiple publics spread across
thousands of geographical locations. The NeGP’s infrastructure *is* the
form that a neoliberalized state in India has taken, made possible
because of the distributed nature of RDBMS.

## Digital Excess

But transition into the digital sphere has been only one side of the
story. Many of the examples I have pointed to above include within them
reports of things gone awry. Of the two million emails received each
day, 80 percent are some form of spam. In fact, the same director of the
NIC mentioned above, runs a team whose sole job is to monitor the
software that filters out spam and prevents it from reaching the email
accounts of government employees. He says most of these attacks come in
from countries with ‘weak or no IT Acts’, such as Israel, and many carry
malware of various kinds, such as an ‘SQL injection’ that corrupts
databases and ‘key loggers’ that copy everything typed onto another
server.[^07NafisHasan_22] Such information, when identified, is supposed to be sent
to the India office of the Computer Emergency Response Team (CERT), but
that doesn’t happen every time. In early 2018, the Indian Parliament was
informed that ‘114 government websites were hacked during April 2017 to
January 2018’.[^07NafisHasan_23] Land record databases are, as we see below, being
constantly reported as compromised. While hacking is used as a generic
term to suggest multiple forms of divergences, the dissonance caused by
the abundant production of data is also felt deeply within the daily
working of bureaucracy in other forms, including errors and breakdowns.

In response to this excess, government agencies are hard at work to
prevent leakage. Cutting across multiple overlapping attempts is the
hiring of armies of ‘ethical hackers’ by the NIC and the renewed call
(for example, in the overarching Personal Data Protection Bill, 2019)
for a return to the localization of data.[^07NafisHasan_24] As a policy, the Data
Protection Bill appears at times almost like a throwback to an era when
organizational and computational limitations had also restricted the
movement of data to local districts. The ‘local’ for the Data Protection
Bill is of course not a subnational administrative unit, but rather the
boundary of the nation. Nevertheless, in laying out rules to *curb* the
movement of data, new policies are retrospectively consciously
constraining the technical possibilities of RDBMS, thereby producing new
political outcomes.

This is hardly the first time that governments have sought to legally
control data movement in the name of security. In addition to
recommending laws (not carried out until this present Bill), ‘third
party audits’ and software logs to track changes made to databases had
been introduced in the past. A common element connecting these myriad
attempts has been the securing of data while *ensuring* its mobility.
The proposed Bill, on the other hand, appears to want to secure data by
*restricting* mobility.

Empirically tracing the emergence of information-as-data in the career
of public bureaucracy reveals the consequences that it has had on the
very existence of the bureaucratic institution. How did we reach a
situation where data becomes unknowable and, in its mobility,
uncontrollable? From static information, stored in registers controlled
by a document keeper, to this onslaught of data – has this gone out of
hand? To trace an implosive, if not regressive, element in the
historical journey of a technology as it got applied to government is
also to diverge from the overbearing, hagiographical, mode of writing
technology’s history in India. As some critiques of science try to do, I
hope to show that along the more familiar, national narrative of
teleological technological modernity, lies a counter story of a
phenomenological crisis in some of society’s most formidable
organizational forms.

## Citizenship as Responsibility: Two Views

My focus so far has been on the effects of RDBMS on the *form* of the
state. But if RDBMS is also *rearranging* the administrative state
itself, what effect might this have on our understanding of a
citizenship premised on state-endowed rights and entitlements? I have
been developing an idea of service as a form of value which the
technical arrangement of RDBMS sets into motion. I intend now to
conceptualize what a service-based approach to *citizenship* might look
like. I do this by
thinking about how technical configurations like RDBMS aid us in forming
neoliberal subjects with particular characteristics, and how this in
turn produces an altered terrain of citizenship: for instance, a shift
from rights to responsibility by shifting older patterns of power by
attributing new technical responsibilities to citizens.

Citizenship has been discussed as rights demanded from the state,
whether as consumers of services or as groups demanding affirmative
action, but less often as *responsibilities* that the state attempts to
place on citizens or citizens on themselves. Projects of development
have often been thought of as collective national projects demanding
contributions from all citizens, and yet the question of responsibility
has not received adequate interest.

Individual responsibility,
self-responsibility, or *responsibilization*, as new forms in which the
governed are encouraged, freely and rationally, to conduct
themselves,[^07NafisHasan_25] are a neoliberal hallmark in which citizenship recasts
itself from a strictly juridical-legal relationship into a biopolitical
mode centered on the capacity and resources of individuals to propel
their own governance. The government, thus, in anthropologist Aihwa
Ong’s terms, applies an ‘optimizing’[^07NafisHasan_26] technique to produce knowledge
of its populations that crucially depends on an ethic of responsibility
among its citizens.

Such an ethic of responsibility, one that
technical arrangements such as RDBMS actively produce, is one of
entrepreneurial governance producing entrepreneurial citizens. The
stories of both people and institutions affected by RDBMS that I chart
here point to a new breed of citizens working at the service of
knowledge production and for a more precise government of the people.
The many engineers, management consultants, computer scientists, and
technicians appearing on the Planning Commission’s horizon right from
the 70s, who continued to become permanent members of the government
system, were also examples of such entrepreneurial responsibility, as
were the business consultants and marketing men who spearheaded RDBMS
into India and who took to multiple channels to advertise its positive
effects.

I have in mind people like Narasimhiah
Seshagiri,[^07NafisHasan_27] who built a network before the internet that could relay
information about planning and development from one corner of the
country to the other, and J. G. Krishnayya, a management consultant, who
went to great lengths in getting the government to adopt a ‘systems
thinking’ approach that could make planning and decision-making quicker.
While pointing to specific kinds of individuals, I am interested in
uncovering a proliferating ethic that rendered the problem of
governmentality into a problem needing technical solutions through
entrepreneurial design. This ethic, I intend to show, arose alongside
the availability of databasing infrastructures: making a
rarely-discussed reconfiguration of citizenship, bureaucracy, and
technology in the redefining of the means of delivering welfare.

Entrepreneurial citizens generate projects that posit new relations
between themselves and those that govern them in the form of an
intervention or enterprise. The entrepreneurial ethic I find in the
people that emerged alongside databasing technologies of governance is
similar to, and yet different from, innovating entrepreneurs such as
those that the computer science researcher Lilly Irani describes in her
recent book.[^07NafisHasan_28] Like her innovators, these entrepreneurs focused on
‘progressive futures *for others* through organizations, know-how, and
resourcefulness’ and have cultivated ‘an ethos of collaboration,
experimental life, empathic civic interest, and the monitoring of
possibility’.[^07NafisHasan_29] Unlike her innovators, the entrepreneurs I describe
were more limited to transforming ‘thinking’ within administrative
structures. Krishnayya, mentioned above, is a great example to think
about the ethic of responsibility that entrepreneurs brought to
government systems. Even before he was officially contracted by the
Planning Commission to help build their systems, Krishnayya had already
begun thinking and writing about what a systems approach to government
would look like. The titles of his papers, which he sent to the
government, sometimes unsolicited, reveal his sense of responsibility
toward ‘improving’ government for a larger good. For instance, his
papers titled ‘Information Services in Administrative Agencies’, ‘A User
Oriented On-Line Computer System to Assist Decisions and Analysis in
Area Development Planning’, ‘Fail-Soft Information Systems in
Government’ were all written in direct and interventionist language and
were meant to provide practical and yet transformative advice on how to
change things for the future. He prescribed both ‘a new philosophy of
information in government’ and ways to operationalize that philosophy
through the design of data and systems.[^07NafisHasan_30] In Section II, I describe the development of this
entrepreneurial ethos, propelled by new techniques of organizing data,
which drove the datafication of a large number of government programs,
from land management to identity and health records.

What we shall also see further on in this essay is a flip side to the
story: excessive digitization and situations of disarray that point to
another kind of responsibilization, marking a different form of
citizenship. This is less associated with grand entrepreneurship and
more with *repairing data affected by digital excess*. As I show in the
case of a land records database, state processes download the labor of
corrections onto farmers, who are then mired in a circuitous process of
correcting errors ascribed to their data. In this process, their claims
on the state vis-à-vis benefits and entitlements is temporarily halted,
making for a shift from ‘thick’ or substantive citizenship to ‘thin’ and
unsubstantiated citizenship.[^07NafisHasan_31]

Such responsibility is not only about keeping one’s data updated, which
would have been the citizen’s responsibility under neoliberalism proper,
but a different responsibility – one that nevertheless emerges from the
fallout of that same neoliberal vision. For the kinds of *labor of
repair* which I describe later in this essay are not bestowed onto
citizens (like rights) but are instead tacitly elided by the state and
its agents and shifted onto citizens. As men and women across the
country are busy repairing their data, damaged as a result of the
excesses of digitization, *citizenship is experienced as a form of
violence*. This is not structural,
spectacular, or episodic forms of violence that scholars of the state
have alerted us to, but what I call a form of ‘slow violence’ given the
slow and concealed way repair creeps into a citizen’s life.

## II

## THE PLANNING COMMISSION’S QUEST FOR ‘DATA IMPROVEMENT’

Many years before data governance came to be synonymous with the
digital, the Planning Commission’s Monitoring and Information Division
(M&I) had begun seriously thinking about an ‘Information System’ that
envisaged nodes and flow of data. The
conceptual and logical work generated around building this system – the
debates over data and its flow – revealed the people in charge of
building the system, their biases and preferences. Most of all, it
revealed their undying belief in technology churning government inside
out, their urge to make its ugly belly transparent, and to reveal the
numerous offices and procedures that the Commission thought did not
work, all to find ways to order and standardize them. Inevitably, the
information system in the Commission became a record of a failure to
stay the course of its mandate.

The failure was evidenced in three different ways in the forecasting and
planning of the Commission’s third annual plan. First, in the
unavailability of recorded information by the ‘sectors’ critical to
planning for the economy referred to as ‘gaps in data’. This related
primarily to agriculture and industries as the two main assets of
economic production in the country. Second, in a ‘time-lag’: in the
unavailability of recorded information in time for the Commission to
make their plans. Third, in a disjuncture between the ‘formats’ in which
information was recorded and sent from the sectors and of the
Commission’s own recording methods – a problem of both ‘retrieval’ and
‘release’.[^07NafisHasan_32] All three added up to an informational crisis, one that
the Planning Commission sought to resolve bureaucratically. The Planning
Commission set up committees, but soon realized the need for technical
consultancy to change the way data was created, digitized, circulated,
and made available to the planning and reporting needs of the
Commission.

The profile of the prosaically named ‘Data Improvement’ Committees now
began to change from career bureaucrats and statisticians to computer
scientists and management consultants. The administration of India’s
future, the archive suggests, was being wired to a network of computers
and their information capacities. Aside from the *zeitgeist* of
computerization in the 70s – silicon bling in dreary bureaucracy – and
the conceptual as well as logistical break from the past that
computerization apparently allowed, it was eventually the limitation of
the technical intervention, the limitation of databasing, that both
defined and curtailed the Planning Commission’s work.

The limitation pertained both to *storage* and *access*. Before Codd had
developed the RDBMS, units of data stored on a computer system could be
traced out only by following a tree-like hierarchy of the system itself
– Folder-File-Data – and were thus dependent on the configuration of the
system, which in turn was under the purview of database administrators
rather than users. This storage method limited its spread and access
because dependence on the computer structure meant editing data could
happen only on the system on which it was stored. At best, data could be
read through remote connections to the storage computer, but this
depended on the speed of the network and also the spread of the computer
nodes, both of which lacked capacity. These limitations pervaded all
decisions. From the prickly question of the centralization of data in
the Commission to its existence in individual departments, from the
meddling of engineers in bureaucratic decisions to the very transition
from paper to the digital, the initial designs of digital stayed close
to the paper system.

In April 1976, the Commission did what possibly no government agency in
India had done before. It sent out a call for proposals to build its
Computerized Data Bank. In a few months, it received detailed responses
from five institutions: the Indian Institutes of Management in Ahmedabad
and Calcutta, the Indian Institute of Technology Delhi, the
Administrative Staff College of India, Hyderabad, and the Systems
Research Institute, Pune. The Commission’s members weighed these
proposals, gave each a sharp but generous review, and eventually
decided, by June 1977, to give up the outsourcing plan altogether and to
construct the data bank itself. That was a bold move for an organization
that had very little experience with computerization, and they did
eventually end up hiring ‘outside’ expertise. For now, at least, the
Commission closed its doors to institutions eager to partner with it.

Yet, J. Krishnayya, the charismatic engineer from Massachusetts
Institute of Technology (MIT) with some years of global IT consultancy
behind him, and at the time the executive director and founder of
Systems Research Institute that had sent the Commission new ideas on how
to modernize its information system, continued to point the Commission
to where it might go wrong with its plan to build a system. Not mincing
his words, Krishnayya wrote an emphatic letter in May 1997 to the
economist Raj Krishna, who had just joined the Commission as a member,
in which he offered critical comments on the data repository that the
Commission proposed to build itself, at least in the initial phases. A
conversation ensued that would point to a lasting problem in the
digitization of information: a problem that was to rankle in
organizational design and would hover over the entire career of
electronic governance in India. This was the problem of the *location*
of data that the Commission was now aiming to centralize into a data
bank. Should control of digitized data rest with individual departments
or should it be centralized in a data bank? If planning by the
Commission was essentially a centralized activity, should data follow
suit? There was also the question of the form that the technology should
take. Should technology *disrupt* the organizational form of government
or should it map onto an existing morphology?

Krishnayya wrote matter of factly that the advice he had earlier given
to the Commission, in the proposal in response to their call, was:

> NOT TO BYPASS the Sectoral Divisions, but rather to link them into a
network \[with decentralized computer equipment\]. The alternative,
which is being followed now, is to construct a large central data bank
administratively in one Division in the hope others will use it. Won’t
happen! People want to control the information they use themselves. It
will be a huge boondoggle eventually, and much wasted effort.[^07NafisHasan_33] 

In their response in June 1977, the Commission defended its decisions:

> The sectoral divisions are not being bypassed, but their information
> needs have been examined separately and an integrated system is being
> developed which would meet all these needs. The inputs for Data Bank
> would be collected and fed into the Data Bank by the individual
> Divisions. The role of the M&I Division is only that of helping in the
> identification, analysis and examination of information needs, design
> and development of the Data Bank, and later, it would be of
> coordinating the operation of the Data Bank by the Divisions
> concerned. It will, therefore, be seen that the Data Bank would not be
> “administered” by one Division but would only be coordinated.[^07NafisHasan_34]

In the inaugural issue of *sacm*, a monthly magazine that Krishnayya and
his colleagues had started in 1979, he defined the problem facing the
nascent attempt at digitizing government as a concern with the
‘application of System Analysis in Government, to problems of
government, and government agencies, in the fields of Industry,
Forestry, Irrigation, Agriculture, Communications, Transport, Urban
development, etc.’[^07NafisHasan_35]

*sacm* aimed, uniquely, to begin a conversation about what would work
for government *per se* without necessarily transitioning ‘solutions’
from the private sector to government. Nothing like *sacm* exists today,
and the fate of that magazine is unclear. It does appear that its
editors had aimed to generate ideas for the use of technology from
within the contours and organizational depths of government itself. They
invited government officers to contribute to the discussion of system
analysis – a phrase that came to be used to describe both IT and
organizational systems. Its inaugural issue, which incorporated papers
from the file on building a centralized data bank for government,
provides a clear description of what system design stood for at the
time.

One essential principle that the editors of *sacm* proposed, for large
computerized information systems in government, was the
*decentralization of data*. This was to them an adequate response to the
decentralized structure of decision-making among government
organizations. This belief came to them from multiple and classic texts
on organizations and system design, such as Katz and Kahn’s 1966
book *The Social Psychology of Organizations* and J.G. Miller’s
1978 book *Living Systems.* Another principle that SRI recommended in
the pages of *sacm* was ‘distribution’, in response to a question of
where information should be processed if it is to be made available ‘at
the appropriate time and frequency and in the appropriate form to
appropriate stakeholders’[^07NafisHasan_36]. The editors defined the different scales
at which decisions were taken as ‘echelons’, saying:

> *Information-processing* capabilities needed to be ‘distributed among
> the various echelons’, depending on (a) the analytic capability
> required at each echelon, (b) the combined economics of processing and
> transmitting information. This meant that each echelon owns a certain
> amount of information-processing capability, though not necessarily a
> mechanized device.[^07NafisHasan_37]

Going further, to show a slew of negative effects of the opposite, that
is, a centralized information system, the editors said that if
centralized,

> the raw data travels a greater distance \[in terms of both time and
> space\]. When the raw data travels more, there could be the following
> consequences: (i) the delays are greater, (ii) more errors creep in,
> (iii) communication costs more, (iv) in general the reliability is
> lower, (v) the context or the relevance \[the metalanguage\] of the
> data may get lost, (vi) inappropriate aggregation may result, (vii)
> reaction time with regard to new data ideas is long.[^07NafisHasan_38]

Importantly, they also pointed to the ‘political consequences of
centralized processing’ in which they said that centralization led to
the concentration of power at the center and a reduction in morale and
decision-making of people in the echelons.

Essentially, Krishnayya’s critique was that the Planning Commission’s
data bank was counterintuitive to how governance in India worked. If the
Commission’s focus was to create a centralized data bank even as they
strengthened the information systems of individual sectors, then its
design needed to understand what kind of storing, retrieval, and
processing of data would happen at which scale. Questions abounded on
the technical capacities and structure of the devices that the
Commission was putting together.[^07NafisHasan_39] While discussing the need for
rephasing projects based on changing commitments and demands, the
Commission notes: ‘How and where the cuts on the past commitments be
affected and how to tailor the present budget accordingly \[…\] is a
problem situation to which an information system should respond’.[^07NafisHasan_40]
In part this drew from Krishnayya’s philosophy that system design be
based on fidelity to organizational forms. There was another reason why
*sacm* was recommending decentralized storage of data: the databasing
capacities available at the time. Technically, *sacm* recommended a
database management system (DBMS), an IMAGE database system for its
QUERY language. They claimed that the IMAGE DBMS was a ready-to-use tool
for information management and hence ideal for a decentralized
information structure. They, therefore, recommended installing the DBMS
on minicomputers, with an RTE-III operating system that had a file
manager, and installing these minis at the same levels as where
decision-making in government was taking place. This, they believed, was
a viable structure, and it would not disrupt the forays that the
government had already made in decentralizing decision-making.

Until then, only large-scale, general-purpose computers had been used
for all information processing applications. These monoliths had
constrained the information system structure to the extent that, even in
organizations where decision-making had been significantly
decentralized, most information processing functions nevertheless
remained centralized. With the rapid advance of minicomputer technology
emerged ‘minis’ packed with powerful features, suitable for a location
with small to medium requirements. Corporate users now had the
attractive alternative of constructing, at all stages, networks of mini
data centers, each equipped with low input/output devices and modular
memory devices appropriate to the information processing echelons.
Distributed minicomputer-based systems further developed the
characteristic of ‘adding-on’ whenever additional processing capability
was called for, thus allowing for possible technical evolution to stay
in step with growing organizations.[^07NafisHasan_41]

The Commission’s centralized data bank inevitably ran into problems. It
could not get individual departments to digitize their data in the
formats that it had created, nor to reengineer their processes in ways
that could streamline the flow of data from departments in the states
and districts to the centralized data bank in New Delhi’s Yojana
Bhawan[^07NafisHasan_42]. Notes from a 1975 annual plan meeting between
representatives from the ‘Industries Sector’, Centrally Sponsored
Programs of the Department of Mines, and the Planning Commission point
to some of the urgency and frustration evident among members of the
Commission. That the Commission found that sectors could improve their
control on the information they generated can be inferred from the
following statement:

> It was significant to note that the distribution of allocations
> vis-à-vis the strategies for project implementation i.e., holding the
> project, slowing it down or shelving it, was being handled through
> negotiations. Given the Data Base the same could have been achieved
> through recourse to a simple linear programming algorithm.[^07NafisHasan_43]

Later, in early 1978, the Commission ran into more problems with
collecting data from the sectoral departments, even in the filling out
of minimum standardized data record sheets. However, even if this had
been sorted out, the flow and access of data would continue to be
severely restricted in the absence of technical infrastructure to
connect to the main computer in which all the data was purportedly
stored. In this regard, some, if not all, of Krishnayya’s ominous
statements about the centralized data bank would ring true.

But just when the Commission’s plans were failing, a new project emerged
in sight. This was the creation of the National Informatics Centre, or
the now-common sight NIC, housed under the Electronics Commission and
partly funded by a grant from the United Nations Development Programme
(UNDP).[^07NafisHasan_44] Since the NIC was a cocreation of the UNDP and
the Electronics Commission, with the blessings of the Planning
Commission, technical consultancy from across the world was being
made available to put it together. An entire file dedicated to the
debates, meetings, and decisions around the planning for NIC reveals the
gigantic infrastructural changes it was bringing to life. UNDP described
it as a project of ‘very great national importance – the scale and
complexity of this project makes it a pioneering experiment’, and went
on to justify NIC as follows:

> A crucial requirement for national socio-economic planning and planned
> management is the availability of an extensive information system
> based on reliable data. Only then does it become possible to develop
> and to analyze policy options by employing, modeling and
> forecasting techniques.[^07NafisHasan_45]

NIC’s ambition was to conceptualize an information design and the flow
of that information through the networks that it built, the most popular
being the NICNET – a network before the internet that aimed to connect
district offices across the country to a center. At first, NIC was less
an organization and more like a network of computers. With the emergence
of the NIC, it appears that Krishnayya’s idea of a decentralized
information architecture that connected departments through a network
was finally being taken seriously. It is, however, most closely
associated with the computer scientist N. Seshagiri, one of its
prominent executive directors. For NIC, in addition to establishing a
supercomputer host in Yojana Bhawan in New Delhi which linked to several
minicomputers in various sectors, there was also the work of building
sectoral or department-wise data systems. This involved digitizing
information in these sectors, and then creating a database management
system for individual sets of data. NIC’s job was to create a
standardized sectoral DBMS allowing sector-wise comparison, even when
the data itself was stored in the Planning Commission’s supercomputer.

NIC launched this project with three priority
data banks, or information systems, for three sectors that the
Commission identified as having a ‘pronounced influence on the national
economy,[^07NafisHasan_46]^ ^namely agriculture, manpower, and industry and
technology. In each, the idea was to create a consolidated sector-wise
data bank. So, for agriculture, information that would be related to
agricultural products, geological data, meteorological data,
oceanographical data, and hydrological data was collected as independent
sets, with the NIC aiming to create a common system for all this data.

NIC’s goal was to achieve standardization by improving the way data
could be classified *across* sectors. Classification of data in a
hierarchical, tree-wise structure, a condition of DBMS, was necessary
for easy retrievability. Ravi K. Zutshi, a consultant at the Planning
Commission, noted that a coding structure was to be devised
for classification that would distinguish between sectors, projects,
and various categorizations that have to be incorporated in the
database.[^07NafisHasan_47] A hierarchical coding structure was developed: (1)
Industries Code; (2) Category Subcode; (3) Project Code; and (4) File
Code. Different projects would then fall under one of these categories
and would be given an individual number. A project code dictionary would
have to be developed to provide easy access to the specific project in
the centralized database. Since a number of files of information would
be associated with every DBMS, a structure to name the files would also
be needed. Zutshi proposed a hierarchy of
‘Sector File-Project File-Company File-Scheme File’. Other
categories, beyond the four main ones, pertained to reasons for
escalation and delay, and included a ‘scarce resource subcode’. Based on
this categorization, project reports were printed out and made available
to the Commission. In this way, data was made mobile in a standardized
and tabularized format. These sectoral DBMS databases were to be hosted
on a main computer in New Delhi, purchased by the UNDP, and linked to
minicomputers in states and districts.

The Commission’s centralized data bank did
eventually take off, but the infrastructural work of creating a network
that would link the supercomputer with the minis, of designing the
format for data storage in the DBMS, and, most importantly, of getting
departments to input data in these formats appeared monumental in
comparison to the amount of data actually transacted. The data bank,
even when up and running, allowed for the transference of only a small
proportion of data (compared to the Commission’s planning needs) and
that too with glitches and delays. So, even when the digital had
replaced the slow and unpredictable flow of paper that had frustrated
the Commission in the first place, and created the need for a
computerized data bank, its success was constrained by the vagaries of
available infrastructure, the creative but tenuous arrangement of a
network that produced only a trickle of data.

There were also political consequences, which resulted in something of a
technical artifice. Organizationally, the NIC was imagined as a
relationship between the Planning Commission and Electronics Commission.
But that relationship was choppy from the very start. There are notes
from Planning Commission members suggesting that the Electronic
Commission, via the people developing the NIC, was trying to go beyond
its mandate and decide what ‘information’ should be generated by the
sectors. They were merely ‘physical technicians’, and it would be ‘odd’
if they gave suggestions like that. Apparently, the noting suggests, the
Electronics Commission was obstructing the development of decentralized
databases by individual departments and agencies.

Essentially, the Planning Commission aimed to create a separation
between the people and the departments that would plan the data to be
collected, stored, and retrieved, and those, such as the NIC, who
implemented these plans by looking after the technical aspect of the
information system. Such a conceptual-technical split has characterized
the politics of NIC’s work with government departments and has over the
years led to a gap between intent and outcome, evident from the
checkered nature of digitization projects in government.

## III

##  

## DATA EXCESS: RELATIONAL DATABASE MANAGEMENT AND DATA PROLIFERATION 

## 

## Technical Specifics of RDBMS

The storage of data from a tree-based or network structure to one of
rows and columns opened up possibilities for the arrangement and access
to data that had not been fathomable before that. In database
terminology, RDBMS changed the way ‘entities’, or pieces of information
about the real world, could be represented and expressed. Such
‘entities’ included ‘real’ or non-digital representations of the world
such as ledgers of land records, and ‘relations’ referred to the
connection between them. RDBMS is, says one writer, a set of ‘relational
database systems—which organize information conceptually in a similar
manner to the tabular layout of a spreadsheet, but with concurrent
access, transactional reliability, and a flexible querying interface’
that ‘ultimately became the dominant technology for storage and
retrieval of structured data in commercial businesses and the de facto
standard on the web’, providing the ‘technical core of a vast, global
transformation of enterprise data processing and management’.[^07NafisHasan_48]

Rather than using pointers between entities in a network relation, and
thereby enforcing some sort of referential link between entities (such
as the hierarchical relation in the DBMS that the Planning Commission
had built in the 70s), storage of data in tabular formats was not based
on prior referential connection, but rather on the possibility of
expressing those connections whenever desired. This difference can also
be understood as the attempt of the networked model to mimic a
real-world physical relationship into symbolic, tabular forms.

These differences between DBMS and RDBMS started becoming apparent to me
as I began meeting database administrators.[^07NafisHasan_49] Most, if not all, were
part of the NIC which has since grown from being a small part of the
Planning Commission into a full-fledged organization. Most were young
engineers who had worked for a few years on contract for the NIC or
elsewhere, and had slowly been elevated into permanent employees. Many
spoke about data security, some about design. In between rough sketches
of tables, my notebook began to carry statements such as ‘design is both
art and science’, ‘a good designer sees the database in his mind before
he sets about building the database’. Called an ‘entity-relation’ (or
E-R) diagram, these young database administrators (DBAs) claimed that
they would use paper and pen to labor over the multiple relations that
now appeared possible between ‘entities’.

Since the NIC builds databases for government departments that already
have some form of storage mechanism in a physical format, drawing the
E-R meant having to understand, from the ledgers and registers waiting
to be digitized and databased, what relations existed between the
entities. Engineers call this ‘domain knowledge’, accrued over many
years of hanging out with staff whose work they aimed to digitize. I saw
this repeatedly across departments. One or two DBAs would have developed
close ties with some staff in the government office and that connection
would seem to power the progress of the database projects.

Once the E-R was established through flowchart-like diagrams, the actual
project began. Unlike a tree or network-based database structure, the
E-R did not determine structure by itself, but instead showed all the
relations possible between entities. Based on these relational
possibilities, the entities were ordered into tables, with other
constraints in mind, such as not increasing the columns of a table
beyond 15. This was the background of tables. The front itself was an
interactive screen that allowed for various combinations of the entities
to be seen. Codd, when pioneering the database
model, had stressed on this feature of RDBMS,[^07NafisHasan_50] and indeed the fact
that people using it did not have to worry about the ordering of the
tables or the E-R relations would be a critical component of its
commercial success.

A critical aspect of this symbolic view of data was the technique of
indexing or pulling up different sets of records and presenting them in
a picture that allowed them to be viewed together in different
combinations. Without indexing, databases had to be queried one record
at a time, defeating the very purpose it was set up for, namely quick
access to different slices of data. Indexes are built using unique
identifiers (or the ‘primary key’ in database language) for every
record. A ‘pointer’ with the location of the record in the disk on which
the database is stored is created, so that querying a record means going
directly to where that record is located. While the index itself is
large, querying times reduce, taking us to the next inevitable level of
multiple higher-level indices, created with pointers to an underlying
index, and then to the data tables. This combined index structure,
allowing a faster search, the addition, modification or deletion of
records, or the ‘B-Tree index’, was invented in the 70s. In Castelle’s
words, ‘without this technique, relational models would likely have
remained as inefficient as their detractors often predicted’.[^07NafisHasan_51]

Such a relational model brought with it new ways of organizing data on a
disk, and newer and faster ways of accessing individual records of that
data. It also importantly brought about an accessible interface to the
‘casual user’ now no longer limited to the programmer and independent
from the structure of the data on the disk. This software interface,
along with larger random access devices (that allowed for many more
locations for storing data tables), allowed for simultaneous work on the
data from different locations, not possible in the prior models. This in
turn enabled ‘on-line transaction processing’ or OLAP, made possible by
the RDBMS defining criteria for online transactions.

The value of RDBMS began to be seen against the acronym ACID. It is
worth understanding what ACID actually means, since this defines the
expectations that corporate organizations have for RDBMS. *Atomicity* is
meant to indicate that ‘individual transactions either occur or – if
aborted – have no effect; *Consistency* *–* the data appears in correct,
valid state all the time; *Isolation –* transactions are isolated from
one another; this is equivalent to the appearance of serialized
execution; *Durability* – successful transactions persist and do not
disappear or become corrupted in the case of failures’.[^07NafisHasan_52]

At the heart of ACID was the desire for a robust system that would
ensure ‘information retrieval’ of rapidly changing entities which
organizational theorists had identified since the 50s as central to
bureaucratic organizations. Yet, it wasn’t information in its entirety
that was needed to be available all the time. Instead, like the
management consultant Peter Drucker said of the business executive,
‘problems have to be presented to him in a form which allows him to act,
that is stripped of everything not pertaining to the business of the
moment’.[^07NafisHasan_53] By making databases ACID-compliant, information retrieval
could happen selectively.

## RDBMS and the Entrepreneurial Spirit

Inevitably, the arrival of RDBMS in India became complicated. Given that
it was specifically designed for commercial use in the US, its adoption
by industry in India matched expectations. But, what of the government?
Did government in India need or use OLAP and, by extension, did it need
the support that RDBMS was intended to provide? Older engineers are
surprised when I ask the question. To them, RDBMS has become so
ubiquitous that it does not warrant discussion. They remember the NIC
switching from DBMS to RDBMS as a natural progression of things, from
the older to the newer. It was hard to get people to think about what
value RDBMS was actually adding to their work. It began to appear that
the significant leap in the digitization of India’s government,
paralleling the growth of RDBMS in the country, was simply viewed in
evolutionary terms.

While this is chronologically true, I shall challenge the assumption
that RDBMS meets the same requirements in government as in the
corporations it was meant for. More importantly, when one pays attention
to *what* is digitized within government and *how* that stands in
relation to its physical form, one finds that RDBMS may not have after
all been employed in government for the reasons for it had been
originally invented. Let us question its efficacy, in relation to the
risk that is posed by digital data, by returning to the instances of
leakage I had introduced at the beginning of this essay.

First, however, a short description of the promises and perils of RDBMS
and the entrepreneurial spirit it gave rise to as it entered India in
the 90s. In several of the statements of its early promoters can also be
read a call for responsibility as a potential for better governance of
the nation. Such a spirit would be further
tied to the arrival of ‘experts’, different from incumbent bureaucrats
and managers, leading eventually, I suggest below in my example of the
digitization of landownership data, to a further weakening of control
over data. Most significantly, it would lead to an ensuing shift in
responsibility – from entrepreneurs to citizen-beneficiaries governed,
in large measure, by new citizenship responsibilities arising from the
excesses of entrepreneurial overattention to digitization.

The ten-year period between the late 80s and late 90s marked heightened
activity in the marketing of RDBMS in India. According to a
NASSCOM study, domestic RDBMS sales went up by 90 percent in 1994–95
compared to the previous year.[^07NafisHasan_54] The 200 firms established by the
mid-80s in the US database industry selling ‘DBMS software, tools, and
related products’, emerging out of the heady California ‘start-up’ days,
were making forays into other markets, particularly in South and
Southeast Asia.[^07NafisHasan_55] Firms like IBM, Oracle, Ingres, Informix, and
Sybase had had an established presence in India by the mid-90s.
Informix, started by a computer engineer at UC Berkeley named Roger
Sippal, tied up with the Indian software firm IDM in 1989, the same year
that it started offering OLAP transactions with Informix Online.[^07NafisHasan_56]
Informix was the first to create an SQL-based RDBMS for DOS in 1986. The
*Times of India* reported this alliance as revolutionary, for it ‘gives
users decision-making powers by offering them access to information
regardless of database location or desktop platform \[…\] helping define
standards that will make technology more accessible and affordable to
users’.[^07NafisHasan_57]

Meanwhile, Sybase, best known for aiding the
computerization of Wall Street in the mid-80s with its RDBMS software
product made exclusively for Sun Microsystems’ client-server
configuration, tied up with Hindustan Computers Ltd., better known as
HCL, to expand their database sales in Southeast Asia. The alliance
specifically offered ‘a Sybase solution along with database consulting,
training and programming services’.[^07NafisHasan_58] Even though it was IBM where
knowledge of relational technology was first generated (Codd was at IBM
when he wrote his pioneering paper),[^07NafisHasan_59] it was Oracle that would be
credited with the commercial success of RDBMS.[^07NafisHasan_60] In May 1991, Oracle
opened a liaison office to ‘coordinate localization for India \[…\] as a
market with a lot of exciting potential’.[^07NafisHasan_61] Its major customer in
India was the government – the Centre for Railway Information Systems
(CRIS), All India Institute of Medical Sciences (AIIMS), Steel Authority
of India (SAIL), and Centre for Development of Telematics (C-DoT).[^07NafisHasan_62]
By 1993, Oracle had set up a fully functional Indian subsidiary, and
Indian companies like Infosys, TCS, and others had begun manufacturing
and selling RDBMS software.

RDBMS was also recognized and circulated as a specific computer skill,
along with programming languages of the day, and advertisements for both
students and faculty were put out regularly.[^07NafisHasan_63] Job calls for
‘programmers and system managers who had experience with RDBMS’ and even
more specifically with Oracle or Ingres, were widely placed for both
local and multinational companies.[^07NafisHasan_64] *Times of India*’s ‘On the Move’
section that tracked hiring and movement of corporate honchos, lists in
1993 the hiring by Datamatics of a general manager for RDBMS.[^07NafisHasan_65] In
editorials, writers waxed eloquent about its transformational
possibilities. Madhu Valluri, a regular contributor to the *Times of
India*, wrote, for example, about how a computer system developed in the
US to track and communicate environmental disasters could provide an
‘insight into what’s actually going on around us \[…\] at a touch of a
key’.[^07NafisHasan_66] Valluri complained that ‘today, not a single state government
has access to instant information about the chemical composition of its
rivers. Neither there is any biological information of its marine
life’[^07NafisHasan_67], and setting up RDBMS systems would enable all of that.

Outside government, RDBMS was deployed in multiple industries –
automobiles (for instance, Maruti introduced Oracle RDBMS in 1994 to
keep track of millions of moving parts in its Gurgaon manufacturing
assembly) and, most visibly, the financial sector comprising banks,
stock exchanges, and other financial institutions. Further examples
include deployment for a ‘screen-based order-and-quote trading
system’[^07NafisHasan_68] for the National Stock Exchange, Delhi Stock Exchange, and
Pune Stock Exchange. In the late 90s, after its success with Finacle,
Infosys created BANCS 2000, an RDBMS for the banking sector offering an
information system and decision support system under one roof[^07NafisHasan_69] that
was later described as ‘a core on-line transaction product operating in
300 sites for 22 banks in seven countries’.[^07NafisHasan_70] 

A specific challenge to the banking sector was posed by nationalized
banks. Tata Consultancy Services was already in the fray for the
automation of nationalized banks, which constituted by one estimate a
market share of INR 250 crore.[^07NafisHasan_71] What these companies offered was a
powerful RDBMS that would conduct the operations of ‘calculation of
demand and time liability, fund and non-fund based advances such as
loans, overdrafts and letters of credit. The software also took care of
remittances, safe keeping operations and foreign exchange
accounts’.[^07NafisHasan_72] Another writer speculated that a computerized system in
nationalized banks ‘should be able to handle five to 10 million customer
accounts and eight to 10 lakh transactions per day and at the same time
provide acceptable response time per transaction’. He recommended a key
technical requirement, a ‘relational database management system \[…\]
providing parallel server rollback and recovery along with features like
two phase commit’.[^07NafisHasan_73] All that was missing was a ‘concerted marketing
thrust’ to get banks to show ‘enthusiasm for computerization’.

This luminous career of RDBMS in private corporations, particularly
financial ones, gave it a veneer of efficacy that was now being sought
to be transferred into the realm of government. As with the nationalized
banks mentioned above, commentators of the time found it surprising that
governments were not adopting RDBMS as rapidly as they ought to have. To
interrogate this roadblock – and thus to also interrogate the assumption
that since RDBMS was ‘good’ for multisited organizations with a
requirement for high transaction capability, like banks, it would also
necessarily be beneficial for government – we need to make a distinction
between *transaction-based* government services operating in multiple
locations in huge volumes (such as the Indian railways online ticketing,
an oft-repeated example) and the daily work of writing, recording, and
filing inside government bureaucracies, the focus of technology-mediated
‘transparency’ reforms (such as the management of land records through
databases, discussed below). While the former lends itself to RDBMS use,
it is the latter that requires us to question RDBMS’ efficacy. Land
records, when digitized, are not transacted online in the same way that
bank functions are, nor is there any ‘intelligence’ generated from their
arrangement in an RDBMS upon which the government acts. A land records
database is as much controlled by a paper economy as the physical
records had once been. These sites, I argue, have also engendered
greater risk of leakage, leading to data excesses.

An example of successful use of RDBMS in transacting services offered by
the government is that of the digitization of the railways booking
system. By the 90s, the Indian Railways Passenger Reservation System
(PRS), one of the largest and most important information systems of the
Indian Railways (itself the world’s largest railway network) had begun
to totter. Even while it was a functioning system, although it had
expanded to computerized ticket reservation, it nevertheless required
visits to the train station or to a PRS reservation office, and often
the assistance of tourist operators. With low-cost airlines offering
competitive prices and easier ways of booking tickets over the internet,
the challenge before CRIS was to make a system on which PRS could be
accessible from many more locations, including the home, and flexible
enough to accommodate real-time updates. In other words, to meet the
‘service’ aspiration of upwardly mobile middle-class passengers.
Unsurprisingly, these demands were believed to have been met by an RDBMS
system.[^07NafisHasan_74]

Yet not everyone was convinced. A top official at CRIS said, ‘the
benefits of emerging from changing over to a RDBMS from the current flat
file system might not be commensurate with the resources expended’.[^07NafisHasan_75]
Other sceptics within the ministry questioned its efficacy, or whether
the need for passengers for ‘more avenues for reservation services’
could have been ‘met without disturbing the core of the system: in fact,
world-wide, major high-volume ticketing systems were still being run on
file-based platforms, rather than DBMSs’.[^07NafisHasan_76] Even as RDBMS in the
railway reservation system has been seen as an important technology, a
minority belief in the department has remained that the volume of
transactions produced with ticket reservation going online with the
Indian Railways Catering and Tourism Corporation (IRCTC) was possible
even without RDBMS. Even so, RDBMS made possible a scale and
distribution of service delivery that had been hitherto unfathomable
before the use of relational systems.

What should be more visible to any researcher of electronic governance
in India, but is rarely the focus of analysis, is where the technical
possibilities offered by RDBMS have produced spillover effects that have
hurt rather than helped the entrepreneurial imagination of governance.
In these situations, RDBMS lends itself to performative impulses that
substitute for the more straightforward practical opportunities that
have defined what we have named the entrepreneurial spirit. From a
purely empirical stance, such situations also depict the
incommensurability of RDBMS for the linear hierarchies of administrative
governance. But its continued and even celebrated uses for these exact
purposes calls for an accounting of its *effects* which, I argue, are to
be found in the shifting terrain of citizen responsibility in and of the
data produced for their governance.

My main example to describe these shifts is the system of land records
management that began to be used from the late 90s to centralize
ownership data with RDBMS. Historically, the recording of landownership
was a colonial enterprise, as has been widely documented. It was usually
the responsibility of village accountants who had custodial control over
their production and maintenance, and who became powerful figures in
village economies as a result.[^07NafisHasan_77] In the late 80s, and following
the World Bank’s belief inspired by claims made by the Peruvian
economist Hernando de Soto that securing property titles could eradicate
poverty, many countries vigorously took up the challenge to ‘clean
up’ their records. Such a cleanup, often powered by the belief that the
physical form of the record was in a mess, sought to digitize the
record, usually in a first phase dedicated to ‘conclusive titling’ of
land, followed by a documentary system that gave owners full and legal
title over land (unlike the present, colonial-origin presumptive titling
of land in India which does not guarantee individual title).
Modernization of land records was closely linked to the belief
that databases could provide the clarity needed to what were
considered opaque practices of record keeping by village accountants.
The concept was first formalized by the Planning Commission when India’s
Prime Minister Manmohan Singh was still its deputy chairman.[^07NafisHasan_78]

In came a number of technology companies aiming to digitize land
records. In Karnataka, Comat technologies first built a Fox Base DBMS
system in the late 90s but then quickly transitioned into an RDBMS when
it became more affordable.[^07NafisHasan_79] The same RDBMS database has existed
since then, and other than offering itself as a digital registry for
printing copies of land records, it has not been used for much else.

None of the original aims – creating a market in land, analyzing the
extent of land types under the supervision of the government, all of
which an RDBMS could enable one to do – have even been attempted. The
printing of digitized records, its primary purpose, had been possible
even with a file-based structure of storing data. In Haryana’s
Kurukshetra, where a database was created around the same time as
Bangalore, the architect, now the director of the NIC in Kurukshetra,
complained that as a young employee building the database in the
RDBMS ‘environment’ there were multiple opportunities for ‘analytics’,
but he had not been given the opportunity to explore any of this.[^07NafisHasan_80]
On the one hand, senior bureaucrats have claimed that land records have
been modernized through technology, and have received national and
international appreciation for this. On the other hand, the undergirding
of this apparent modernization with RDBMS has not been exploited
to perform any kind of analytical work on the records. The irony of this
is not lost on observers, who point out that India’s prowess in IT does
not seem to be applied to its modern land records.[^07NafisHasan_81] In essence, even
when land records *were* digitized, their production was never separated
from the dense practices of paper-based verification and authentication.
The figures and numbers seen in the database are only the symbolic
representation of an intricate process of record creation
located between the field and the office.

## Locating Excesses of Digitization in the Structure of RDBMS

Even while RDBMS databases have not made land governance more
‘intelligent’ – arguably the key purpose for which these databases were
set up and aggressively marketed – has it made the *management* of that
data more risky? In this transition from records in physical registers
to records on a database, multiple aspects of control have been
compromised. First, the already existing gap between what is actually
happening on a piece of land and what records signify has only further
widened. The reason usually lies in the very processes that had brought
database to life for, even as databases marked a disjuncture from the
practices of village accountants, its original architects depended on
those very accountants to verify the first version of digital records.
They were often nothing but physical records typed by young men
and women working on poorly paid contracts for the government.
Verification took so long that the status of the land had often changed
by the time digital records were finally approved.[^07NafisHasan_82] Far from
becoming intelligent, the quality of information in fact suffered, not
to mention the copious amount of time invested in sorting out these
errors.

A second, more technical, question lay around storage and access, and
the potential for manipulation. The RDBMS for land records in Karnataka
includes an entity called ‘surnoc’ or survey number character denoted by
a ‘\*’. This asterisk had been included in the database as an identifier
for the first parcel of land split from a bigger plot. For instance, for
survey number 32, if a *hissa* or split is recorded by one of the joint
owners, the first split gets survey number 32\* to differentiate it from
the original number 32. This convention was originally created when the
database was built, and it was discovered that previously split land was
not being given a separate record. What the database architect didn’t
consider was that putting in a \* for any survey number in the database
– that is entering a \* in the surnoc column – generated a *new*
legitimate record that could be legitimately used for legitimate
transactions.

A senior bureaucrat explained how in an office in his charge, a series
of such offenses came to light when a new database operator accidentally
gave a farmer the ‘wrong’ version of the record, that is, a version
created by a ‘surnoc’ or duplicate to an original survey number. On the
basis of this new record, the unscrupulous operator, according to
the bureaucrat, took loans that the farmer was shocked to now discover.
On hearing this, the bureaucrat telephoned the main operator manning the
centralized database and asked him to dig out all cases in which new
false records were created using the surnoc. A litany of cases emerged,
operators were fired, and conniving village accountants slapped with
criminal cases. The bureaucrat ended this story by saying that this
problem has now been fixed by another new and more tech-savvy
commissioner of land records in the state. 

These were only some of the instances of the many problems that RDBMS
databases had created. Even with the new commissioner, multiple cases
arose of ‘breaking into’ the database to make changes. A case was
reported in 2018 in which 19 acres of government wasteland
were transferred to a private individual.[^07NafisHasan_83] The report also claimed
that it was the third reported time such a ‘breach’ had occurred
in which government land was transferred to private people. It is
interesting that the commissioner chose to respond by differentiating a
‘breach’ from a ‘hack’, saying that the ‘Bhoomi software cannot be
*hacked* at all’[^07NafisHasan_84] and that ‘in both cases, some person has
*breached* the security and logged into the system to change the
database’.[^07NafisHasan_85] It could not be hacked from outside the institution
because it wasn’t online (there has only recently been some move to
create an online database for Bhoomi), and not because there was
anything inherently insecure about it. In the literature, a ‘security
breach’ includes ‘*unauthorized data observation,* *incorrect data
modification, and* *data unavailability*’.[^07NafisHasan_86] The records in Bhoomi
have been found to be replete with missing information – discovered, on
several occasions, in different versions of records printed at different
points in time.

More importantly, the commissioner’s remarks obscure the fact that it
was the very village-level records in their physical registers, and
their process of being databased and stored in the subdistrict, that
created the conditions for this violation. Databasing by its very
nature, and particularly RDBMS with its tables and easy format, provides
the opportunity to access and change data. In database terminology, such
kinds of invasion are called ‘direct attacks’ as ‘the attacker can
easily attack the database as it does not have any protection
mechanism’.[^07NafisHasan_87] The not-so-user-friendly file-based structure of the
database is often more secure against intervention, an unintended
consequence of design since a user needed to know the structure of the
database in order to access it. In RDBMS, on the other hand, any access
to the SQL program that interfaces the data behind it also allows access
to database tables.

One way of securing such access was by introducing an encryption key
that made the data unreadable, as the commissioner eventually said about
the land record data under Bhoomi: ‘As a first step, we are encrypting
the whole of Bhoomi data. This will prevent even officials from seeing
the database’.[^07NafisHasan_88] Encryption has been a long-standing method for
securing data in RDBMS, the literature pointing to many kinds of tools
and techniques for such encryption to prevent ‘intrusion’.[^07NafisHasan_89] There
have also been critiques of encryption itself, such as the argument that
it can ‘significantly degrade the system performance and application
response time’.[^07NafisHasan_90] Encryption remains at best an incomplete solution
to the basic problem of ‘security threats’ that Geertz and Jajodia
suggest arise from the following basic fact:

> Today’s often mission-critical databases no longer contain only data
> used for day-to-day processing by organization; as new applications
> are being added, it is possible for organizations to collect and store
> vast amounts of data quickly and efficiently and to make the data
> readily accessible to the public, typically through Web-based
> applications.[^07NafisHasan_91]

Scholarship on data security often starts with such observations: ‘As
organizations increase their reliance on, possibly distributed,
information systems for daily business, they become more vulnerable to
security breaches even as they gain productivity and efficiency
advantaged’.[^07NafisHasan_92] Even though Bhoomi does not (so far) operate on the
web, its data is spread across databases connected via leased lines
located in multiple subdistricts, and there are plans to connect them
into a centralized web-based architecture. In this situation, encryption
is admittedly a way forward, but it has its limits.

Data finds new locations with RDBMS, even as concerns for data security
recommend limiting ‘access’ points or making the data unreadable through
encryption. This ability of data to be located in multiple locations in
the same tabular formats allows for *an imagination of modularity*,
alongside a *replicability of homogenous form across varied contexts*.

Such an imagination would, in 2006, undergird the ambitious NeGP: a
densely packed policy for digitizing all government administration and
services across many domains of life. The NeGP is often seen as having
brought together a trinity of material forms in its effusive
modernization project. Called ‘core IT infrastructure’, this included
leased internet lines integrated into a State Wide Area Network or SWAN
that offered high speed connectivity between web applications offered at
CSCs but which were actually stored in SDCs. This was an institutional
arrangement for the maintenance of databases and networks at a single
fixed location in the state capital. Front-ends of the application,
producing say birth and death certificates available at CSCs, would be
produced through SWAN’s link to a back-end linked to a data center in
the state capital. All this operated entirely on a client-server model
enabled by RDBMS.

A guidelines document lists several features expected of RDBMS for
developing applications stored in SDC. The RDBMS should, it says,
‘support data base partitioning and parallel processing’, ‘have support
for generation, consumption of XML data and XML based query
capabilities’, ‘allow multi-dimensional OLAP capabilities for Data
Warehousing’.[^07NafisHasan_93] It further suggests that the RDBMS should adopt
industry standards to ensure interoperability between databases.[^07NafisHasan_94]

A couple of years after RDBMS began to be employed for applications, a
study conducted by two computer scientists for 14 e-government services
in the state of Himachal Pradesh in north India in 2010 concluded that
‘the development of e-government applications invariably lacks
conforming to standard database design parameters’.[^07NafisHasan_95] They found
several problems of multiple parameters of database design, important
among them being the absence of primary or foreign keys which greatly
reduced the ‘referential integrity’ or the validity of the relation
between two tables, absence of a ‘constraint mechanism’ to verify data
that can enter a database and ‘poor E-R design’ that pointed to the fact
that databases had not ‘developed any conceptual schema and databases
are designed on ad hoc manner’.[^07NafisHasan_96] The last two aspects pointed to
reduced security measures in the databases, as unverified data entries
and poor E-R design could make databases open to breaches or attacks.
Many of the databases were made by the NIC in Himachal Pradesh, and it
is possible to find similar problems with databases in other states as
the NIC is known to share its design principles.

## Repair of Data and the ‘Slow’ Violence of Excess

That databases being built for government are falling short on design
and security is one aspect of the problem. A more trenchant issue is the
‘breakdown’ of data produced by the *excess* of the technical structure
of RDBMS, as we have seen with Bhoomi. A significant and under-discussed
aspect of this breakdown is the labor involved in the repair and
correction of data, and the way such labor has been shifted onto the
citizens. Claims to citizenship through access to rights and
entitlements depend increasingly critically on this responsibility of
repair, so that for many people citizenship is experienced only through
the practice of data repair.

This is not the same as the neoliberal impulse of responsibilization,
where citizens keep their data updated in their own best interest. What
I am trying to point to is an unintended fallout of this impulse – a
fallout of precisely the opportunity promoted by RDBMS, through
technologies of government to sort out citizen-subject relations in a
discrete and transactable fashion. Just as claims to rights and
entitlements are made unequally, repair too is practiced unevenly. This
is not a problem of capacity, rather it is the concealment of data error
within ongoing material disruptions between citizens and states.
When citizens are required to bear the
responsibility of repair, it is not a visible transfer of
responsibility, rather it is a tacit, neglected, fringe encounter,
embroiled within ongoing material disruptions between the citizen and
the state.

Before I turn to the empirical example to support all that I am saying
here, let me propose one final outcome of this form of unintended
responsibility emerging from relations produced *through* the very
technical opportunities that RDBMS offers. Violence, disaster, and
breakdown are familiar experiences when negotiating with states.
Experiencing citizenship-through-repair is often not a spectacular
crisis or disaster, nor is it a stark infrastructural breakdown or the
choking of infrastructural time. Repairing data is instead best viewed
as temporal vacuity, a state of limbo, a temporary break from ongoing
relationships. It is not structural violence in the usual way of
describing state procedures (though there is some overlap). Nor is it
spectacular violence. I propose to think of it as a temporary,
circuitous low-grade suffering, and so a form of ‘slow’ violence that
scholars have begun to attribute to the slow-moving temporalities of
suffering.[^07NafisHasan_97] *Such violence of data repair, as a mechanism of
citizenship, is slow because it proceeds at a speed that distances
suffering from its original causes*. Repair is embedded in familiar
structures so that citizens are unable to any more distinguish the
repair of data from the other bureaucratic processes within which they
are often mired.

I continue, as I now explicate this pattern of digitization and data
repair, with my example of land records digitization and its
database-driven excesses. We turn now to the repair work that goes into
data rehabilitation. The split experienced between the digital record
itself and the paperwork that continues to surround it is experienced by
farmers as a form of harassment – often physical, involving multiple
trips to offices, courts, hiring and paying advocates, waiting for
months sometimes years to have their errors resolved. It produces a
growing disjunction between the overt promise of transparent, speedy,
and clear databases, and the substantive experience of vacuity produced
by the errors – a form of ironic, symbolic violence.

A few pointed out that people have been urged, since the turn of the
millennium, to become ‘e-citizens’, to conduct their business with the
state online. Encrypted, barcoded, digitally signed land records can be
printed out from internet cafes boasted a young engineer, a
Bhoomi* *consultant. But, as often is the case, when it was revealed
that the record has something amiss – a name wrong, the extent of land
incorrect, missing information about the crops on land, in essence a
record paralyzed in an identification-based ecosystem of entitlements –
people were asked to go back into the dreary world of paper records and
fish out from the dense physicality of the paper record room the claims
about who you are and what you own.

The rehabilitation of these digital errors opens up another side of the
process, namely the administrative-legal procedures of record keeping
and record rehabilitation. In order for an error to be corrected, it
must first be made legible to the bureaucracy. This is done by
reinscribing it as a ‘dispute’ between the owner of land and the head of
the office to which the record belongs. A dispute calls for a specific
arrangement of documentary material with specific inscriptional work,
described below.

Once presented as a dispute, it is put through a revenue court process
in the office of a senior bureaucrat, higher than the head of the office
in which the error, now renamed dispute, is lodged. The court process
takes its own discursive path, ending up in an order that either accepts
the applicant’s request for correction or rejects it by asking for
more supporting documents. If accepted, it comes back to the office
where a ‘mutation’ process begins to make changes in the digital record.
This entire process points to why a digital error cannot be corrected
digitally, since an error is not identified simply as a
typographical error and thus becomes a much more complex legal problem.

A specific feature of the correction process is that the law, on which
the bureaucratic process is based, makes it incumbent on the *owner* to
prove to the bureaucrats that there is indeed a correct version of the
data that is identified as erroneous. This is irrespective of the source
of the error. The effects of such a transfer of responsibility were made
starkly apparent to me in a conversation between an owner and a Bhoomi
operator who had just made an error on his application for change in the
record. The operator had incorrectly entered the wrong name for a
particular record, and the application had now left her ‘login’ which
meant that she could no longer edit it. As part of the state
government’s ever-evolving strategy of gaining further control on the
production of the record, deleting an application at the office level
was not an option any more. When the next bureaucrat in Bhoomi’s
workflow sequence received it and verified the owner’s name on the
screen with what was in the copy of an older paper document, the *Aakar
Band* provided as part of the application, she marked the application as
an error. At this point the application left the ‘mutation’ flow and
went into a ‘dispute’ list of cases that now needed a scanned court
order to be put back into the mutation process. The owner in question
was, in the operator’s words, ‘scolding’ her for making this mistake as
he would now have to run around to have it corrected. The owner bears
the brunt of the state’s centralizing logic that, as becomes further
evident, draws heavily on a colonial logic in which an owner’s rights
are presumptive on her ability to prove at every point in time that her
records are indeed correct, in order to continue to validate the
authenticity of the record and thus to produce the ethos of fairness and
transparency attached to data transaction.

The correction of records often involves chasing files in a circular
fashion as they move within multiple government offices and as clients
move from office to office. Not every record holder makes all these
trips in person. Sometimes these are mediated by brokers or advocates
who represent record holders in revenue courts, or by office clerks
themselves for a fee. Essentially, record holders have to strike a
balance between bearing the burden of running around by themselves at
the cost of losing out on working on their farms or paying bribes to
have it done for them. This depends on the socioeconomic status of the
owners, with rich landowners (identified locally as people owning 15-20
acres of land) being able to afford bribes to hire mediators to do the
job. How soon a dispute will come up for hearing depends on how
networked the advocate hired is with the office clerks and how much
money the record holder is willing to pay to get the job done. Even when
admitted, cases take multiple hearings to finally produce an order. The
magistrate sometimes asks the record holder or his representative to
return with more documents to bolster the file. Building a file becomes
an accretive process, and the only way documents are accepted is through
physical submission to the magistrate.

The Bhoomi operator, whose case I described above, said that
‘caseworkers’ – clerks of the processual side of bureaucracy – do not
work on these files quickly enough. For them it is often merely a ‘drop
in an ocean of files’, and they need to be adequately compensated for
the job. Once an application is marked as ‘dispute’, it falls out of the
First-in-First-Out (FIFO) system (a much-advertised feature of Bhoomi),
after which it depends completely on the whim of the caseworker. There
is no accountability mechanism to track when an error file will come up
for hearing and resolution, thus making people visit offices multiple
times to check on the status. Court sessions are often cancelled because
the office head is busy with other pressing work, but there is no way
for record holders to know that unless they read the notice board. As a
result, offices teem with large numbers of record holders hovering
around the desks of office clerks in charge of handling the correction
file, or in front of the court room where, in performative fashion, the
head of the office will receive documents from them to add to their file
as proof of their ownership.

For citizens, repairing Bhoomi data and thereby recovering their status
as claimants of substantive citizenship (as opposed to legally ascribed
thin citizenship) requires stepping back into the quagmire of paper
bureaucracy. Here is where the first kind of entrepreneurial
responsibility, of the kind that technical configurations such as RDBMS
have spurred, trails off and the burdensome responsibility of the
citizen emerges. The digital service of maintaining land records is put
on hold until resolutions are received. This is a critical moment of
reconnection with a past that had been ostensibly discontinued when the
storage and dissemination of records had been made digital. The
back-and-forth between owning data and being a legitimate subject of
citizen services, and being saddled with the burden of repairing data
and losing that status, depicts the experience of slow violence emerging
in these interactions.

## IV

## 

## CONTAINING EXCESS OR RETURN TO THE LOCAL

One startling aspect of the proposed Personal Data Protection Bill in
India in 2018 was its suggestion that the movement of data be curtailed
by compelling organizations to store data *locally*.[^07NafisHasan_98] The Justice
B.N. Srikrishna Committee report on data privacy says: ‘A policy of
storage and processing of personal data within the territorial
jurisdiction of a country is advocated to ensure effective enforcement
and to secure the critical interests of the nation state.’[^07NafisHasan_99]

‘Local’ here meant *national*: that is, data produced in the country
should remain in the country. If this becomes law, it will
singlehandedly upend the relationship between technological
infrastructures and globalization. There are many technologies of
globalization, and databases are one of them. As Benjamin Baez argues,
databases are ‘informational technologies leading to a new communication
system, one increasingly speaking a universal, digital language and
integrating globally the production and distribution of the words,
sounds, and images of our culture’.[^07NafisHasan_100] In other words, databases are
what make movement from local to global possible. Recall that RDBMS was
a commercial success because it was marketed as a solution to the
problem of organizational spread *across* geographies. In Grier’s words,
‘Codd developed a structure that allowed business people to focus on
certain kinds of relationships. These relationships determined how
businesses thought about their customers, their bills, and their
employees’ *across regions*.[^07NafisHasan_101] In fact, Grier compares the
organization of the World Wide Web to Codd’s relationship structure: ‘It
\[the Web\] was clearly built upon the ideas that Codd developed. Those
ideas could be seen in the databases that supported the Web,
spreadsheets, and even in the organization of data scratched hastily on
a pad of paper’.[^07NafisHasan_102] If RDBMS (or other such technological
infrastructures) are now restricted to national borders, the change they
will inevitably undergo is right now unfathomable.

Going ‘local’ is the Indian government’s most aggressive strategy yet to
prevent what I am calling ‘excess’, but it is definitely not the
instance where the state has tried to comprehend data security. At the
heart of data localization is the question of whether security is
inherently related to the physical proximity of data. What distinguishes
the Indian government’s past attempts at data security has been that
control over data has actually *centered on its mobility, not its
containment*, arising from the foundational concern for keeping
*movement* of data alive. Whether it was in the calls for legislation to
counter the risks of data theft as early as the 70s, as I discuss below,
or the development of a multination standardized framework for
conducting information technology audits in government, security has
been thought of in terms of speed and mobility of data. Calls for
localization as a form of containment in a bid to counter excess can
transform the entire attempt at digitization that this essay has tracked
since the mid-70s. In this section, we trace past attempts at securing
data against excesses to point to different strategies employed, by both
state and non-state, and contrast these with the present attempt at data
localization. This is not an argument either for or against data
localization, rather it shows how, in returning to an imagination of
immobility of data when it exists in physical registers, we are seeing a
return to an earlier imagination. This return is even more startling
when viewed against India’s ongoing history of securing data through
emphasizing mobility while searching for ways to limit excess.

A starting point for tracing the genealogy of the government’s concerns
with data security could be the early years of information digitization,
in the late 70s, when multiple government agencies first began
experimenting with centralized data centers. A seminar conducted at the
Indian Institute of Public Administration in 1979, perhaps the first
time that security threats to India’s steady march toward digitization
were discussed, opened with an evocative lecture on the perils to
privacy. Justice Krishna Iyer, who would retire the following year as
judge of the Kerala High Court, made an emphatic appeal to his audience
(whom he addressed as ‘Scientists, Sociologists, Administrators and
Friends’) to think seriously about the security of data: ‘The problem
before us is temporal – how to tame and train electronic power for the
Human Cause but this is also a problem of value judgement and moral
consciousness – a profound commitment to the dignity of man and progress
of the world community.’[^07NafisHasan_103]

The need for data’s *transcendence from the territorial* – which the
authors of the Personal Data Protection Bill today suggest needs to be
curbed through a legal prevention of the flow of data – is already
identified in this early talk by Krishna Iyer. The threat of security
emerged from the fear that data may go out of hand, leading to a
situation of data excess:

> The consequence of the combined achievements of the computing and
> communications technologies is that data collection and transmission
> is becoming massive in its quantity and apparently limitless in its
> capability. Its speed increases as its cost diminishes. Unrestrained
> by law, it will know no national borders \[…\] the notion that the
> State can control flows of information, difficult enough with paper
> and manual files becomes more difficult with instantaneous
> transmission of information through computer terminals in other
> countries.[^07NafisHasan_104]

Even so, Krishna Iyer did not recommend localizing data in the way the
Personal Data Protection Bill recommends. His expectation from the law
was to provide what he called ‘pre-emptive action’ against attacks on
security, sometimes belied by his distrust of the ‘average lawyer and
judge’ whom he considered ‘illiterate about designing privacy
legislation suitable for the computer age’. Nevertheless, he believed
that strong legal safeguards for security was the only way forward.

It is an irony that having given this lecture at the very beginning of
the massive digitization attempts of the Indian state, Krishna Iyer
would, toward the end of his life, fight a bitter war against Aadhaar
for breaching personal security.[^07NafisHasan_105] What followed, in the years after
his lecture, were state-led interventions for instilling security that
ranged from creating committees and reports to hiring ‘ethical hackers’.
Soon after Krishna Iyer’s lecture, in 1980, a Committee/Panel of
Specialists in the Department of Electronics, set up in the Electronic
Commission to advise it on ‘problems of ensuring security of information
while using electronic data processing (EDP) equipment’, submitted its
final report.[^07NafisHasan_106] The report consisted of the work of six working
group committees to draft guidelines on various aspects of security.
These groups included members from the NIC, the Intelligence Bureau, the
army, scientists from Tata Institute of Fundamental Research (TIFR), and
civil servants. The report that they produced was detailed, covering
multiple aspects of data production and communication. But as a Special
Invitee to the final meeting of the committee from the Ministry of Law
and Justice pointed out, data processing activity in India in general
was at an early stage and depended heavily on the experience of the
West, discernible from the list of references. The language used to
justify the report seemed, he appeared to suggest, out of place with the
nascent nature of database development in the country. In hindsight, we
may now infer that this was possibly only appropriate to the later
moment of RDBMS development. It said, ‘shared resources and jointly used
data have become the normal mode of computer operations’, which made the
issue of data security or ‘the protection of data against unauthorized
disclosure, modification, restriction, or destruction’ especially
critical.[^07NafisHasan_107]

The synchronous use of data was hardly a feature of the databases
operating in India at the time. Neither was a ‘direct interaction with
computer’ – once the prerogative of the programmer or operator, now a
‘common place activity for the most casual of computer users’ – much in
evidence.[^07NafisHasan_108] It appeared that data security in the 80s was seeking
solutions to problems that had not yet arrived. Even so, there was
detailed focus on the problems arising from making data mobile, as
members of this committee braced themselves for the excesses of data
that they realized would soon arise from the multiple paths that data
would traverse across the country. Under the subsection ‘Data Base
Security and Communications’, the report explained:

> When multiple users are accessing centralized data through terminal
> devices from remote locations linked to a central computer system via
> telephone lines or other communication links, a number of security
> problems arise. When we have to deal with a large population of users,
> massive amount of data, many communications links and a vast array of
> functions \[…\] safeguards are necessary.[^07NafisHasan_109]

This was before the internet, and so the committee focused on dial-up,
leased, satellite, or radio microwave links. Their focus on how to
safeguard these communication links remains valid, for data for many
e-governance projects continues to be sent on leased lines, both to data
centers and to front-end locations. They envisaged the role of both
Posts and Telegraphs and of Telecommunications to be one of ‘ensur(ing)
security of data which will traverse the communication links between the
men and the computers’.[^07NafisHasan_110] Much of the imagined movement was through
‘switched communication links’ which ‘pass through the public telephone
exchange network’ or a ‘dedicated communication link’ which offered a
‘dedicated line between two or more computers or between a computer and
a remote terminal, using data modems’.[^07NafisHasan_111] Securing the former was
considered difficult, since movement depended on large number of people
(telephone operators) and did not involve more than physically locking
the ‘cabinets’ (nodes through which data passed).

In sum, the report envisaged a situation of data mobility through the
infrastructure of the time and recommended ways by which such existing
infrastructure, like the telephone switch system, could be made more
secure. It also made a few generic recommendations about securing the
operational apparatus, such as physically securing the site of
operations, creating access protocols for personnel, backing up computer
hardware and data tapes and discs, and classifying data depending on the
security risks they pose and the mechanisms to control access. The
report dedicated a few pages to laying out risk, recommending
‘Communications Line Safeguards’ as against ‘penetration techniques’
such as ‘masquerading’, ‘eavesdropping’, ‘piggybacking’ and ‘Line
Grabbing’. The focus was on securing data as it travelled across sites,
and it forewarned the breaches and attacks that government data could
suffer (and indeed did suffer in the decades that followed).

A third, and more direct, involvement with managing the risks associated
with data has been the government’s investment in auditing the
infrastructure of digitization, including software code and data banks.
Here, too, the focus was not on curtailing the movement of data, but on
checking for risks in a limited way.

For digital infrastructures, an ‘audit’ includes common physical and
selective checking, but also includes specific digital interventions
such as maintaining automated audit logs to connect movement of data
with users. The physical auditing of data is part of every digitization
project that the government undertakes every time manual data transforms
into a digital platform. In the digitization of land records in
Karnataka, for example, digitized data was, we saw, made online only
after its verification by village accountants, and in some cases by
district commissioners, sometimes causing problems such as how to keep
the database ‘live’ and in sync with reality. Even so, physical audit at
the moment of transitioning from manual to digital continues.

A second kind of audit practice is the recording audit logs that track
the history of change made to the data in the database tables. This, as
a NIC DBA explained to me, is a critical component of the database, to
track what changes have been made to core data and by whom. DBAs usually
store the audit log in a separate table that contains columns for user
id, IP address (to track from where the change was made), what changes
were made (addition, deletion, modification), and the exact time at
which this was done. This table is usually accessible to the ‘super
admin’ of the database. Sometimes, to get around server space
constraints, audit logs are stored in a separate database and a ‘dirty
flag’ is used to highlight changes. A claim that I heard repeated
several times by people critical of government databases is that they
didn’t maintain robust audit logs, making the breach of government
databases not so difficult. In any case, audit logs seem to be a
critical component, applied across the board, of maintaining security
within databases.

A fourth type of audit practice that has emerged after the digital
infrastructure of the NeGP is of third party auditing or TPA,
particularly of the SWAN. This emphasis continues the focus on securing
communication links from the pre-internet days, and is on how to ensure
both mobility and security. Even some of the language is the same, of
‘penetration testing’ and ‘vulnerability testing’. The difference with
older attempts is that large private corporations are involved in both
creating of the network and its security management.

According to a Request for Proposals for the selection of a TPA:

> SWAN (State Wide Area Network) is envisaged as the converged backbone
> network for data, voice and video communications throughout the
> State/UT and is expected to cater to the information communication
> requirements of all the departments. Key focus of the SWAN project is
> on high service delivery. As per SWAN policy, all States/UTs are
> implementing SWAN under two Options. Under the first Option, the State
> is to select a suitable Public Private Partnership (PPP) model and get
> the SWAN commissioned and operated for 5 years by a private Network
> Operator. In the second Option, the SWAN for the States/UTs would be
> set up and operated for 5 years by the National Informatics Centre
> (NIC). In either of the Options a Third Party Auditor (TPA) is
> required.[^07NafisHasan_112]

The document then outlines the work that a TPA will be expected to
undertake:

> Third Party Audit shall include monitoring the performance of the SWAN
> with a view to ensure desired Quality of Service (QoS) by the Network
> Operator and bandwidth service provider, as defined in the respective
> SLA’s, signed between the State/UT Government, and Bandwidth Service
> Provider, Network Operator. These Guidelines define the broad areas of
> work, which TPA shall perform for a period of five years from the date
> of final acceptance test of the network.[^07NafisHasan_113]

PriceWaterhouseCoopers or PwC is, for example, a popular TPA in many
government departments, though other firms also compete for that
position. Bureaucrats generally take pride in naming these companies.
Beyond physical verification, database audit logs, and employing third
party vendors, some national organizations are also involved in the
creation of audit protocols which were applied across multiple
departments. The Comptroller & Auditor General (CAG) of India is a
‘supreme audit institution’ or SAI, one of a set of government audit
institutions around the world. As a SAI, it has led a cross-country
working group on IT audits since the 80s, through which, a senior
director of a NIC told me enthusiastically, it has been auditing data
quality, the process of data entry and data validation of major
government schemes such as the National Rural Employment Guarantee
Scheme (NREGS). He added that government departments are happy with
CAG’s involvement because they have an oversight on the NIC.

A handbook published on IT audit by the working group states the need
for such audits as a:

> natural response to the increasingly computerized operations of
> governments and public sector organizations. While the increasing use
> of IT has led to improving business efficiency and effectiveness of
> service delivery, it has also brought with it risks and
> vulnerabilities associated with computerized databases and business
> applications, which typically define an automated working environment.
> The role of IT audit in providing assurance that appropriate processes
> are in place to manage the relevant IT risks and vulnerabilities is
> crucial if the SAI is to meaningfully report on the efficiency and
> effectiveness of government and public sector operations. In the IT
> audit environment, processes, tools, oversight, and other ways to
> manage a function are also referred to as controls.[^07NafisHasan_114]

The objectives of the CAG audit are related to data integrity, by which
they mean the data that is used in decision-making and operating
organizations’ core function. An ‘audit can definitively identify risks
to data integrity, abuse and privacy, and also provide assurance that
mitigating controls are in place’.[^07NafisHasan_115] The focus on integrity is in
the service of ensuring mobility. The handbook points out that computers
today communicate with each other and exchange data over networks, both
public and private. It also acknowledges that:

> employing overseas service providers is a common form of outsourcing,
> especially in a cloud computing environment, even though this poses
> risks involving foreign regulations on information storage and
> transfer may limit what can be stored and how it can be processed,
> data may be used by law enforcement of a foreign country without the
> knowledge of the organization, privacy and security standards may not
> always be commensurate, and disputes because of the different legal
> jurisdictions cannot be totally avoided.[^07NafisHasan_116]

But instead of clamping down on overseas data operations, it recommends
a ‘strategy on contracting services to overseas vendors’[^07NafisHasan_117] which
asks the organization to make itself aware of overseas laws and
regulations, reports on a vendor’s past performance, and on ‘deviations
from the Service Level Agreement and outsourcing contract’[^07NafisHasan_118] among
other things.

In all these instances, we see actions dedicated to data mobility rather
than its containment. They give us a new vantage point from where the
current calls for the localization of data in order to secure it might
be viewed.

To summarize the main arguments of this essay. The phenomenon of data
excess, and its effects on the ability of governments to control
information, is linked to the emergence of relational databases (among
other technologies like networks), which have created infrastructure for
data proliferation without necessarily ramping up expected efficiencies
such as those produced in the corporate sector. Instead, the phenomenon
of data excess forces citizen-beneficiaries to engage in repairing their
data, producing moments of vacant citizenship, a situation I term ‘slow
violence’.

The examples I have provided in this chapter are of classic
bureaucracies (the bureaucracy concerned with land has been my chief
example) that have undergone a significant change in their
information-producing capacities with the introduction of RDBMS. Classic
forms of bureaucracy have been described as ‘a remarkable form of human
organization that has enabled modern governments and corporations to
provide previously unimaginable benefits to humans around the
world’.[^07NafisHasan_119] The question that the disruption in the flow of data that
RDBMS poses is whether the organizational form of the bureaucracy will
survive in the way it was imagined. In other words, in a networked
digital age, does bureaucracy remain an efficient and effective
apparatus for managing human affairs if its control on the information
it produces is weakening?

Multiple bureaucrats in the land bureaucracy in Karnataka told me that
after the land records went digital, the bureaucrats know *less* about
the lands under their jurisdiction. Digital records have proliferated,
but not necessarily aided bureaucracies in control. Is declining
governmental effectiveness punctuated by disastrous events like a data
breach, an outcome of the digital transformation that has been sweeping
government since the Commission built its first centralized database?

[^07NafisHasan_1]: ‘Over 22k Indian Websites, 114 Govt Portals Hacked between Apr
    2017-Jan 2018’, 7 March 2018,
    https://www.business-standard.com/article/current-affairs/over-22k-indian-websites-114-govt-portals-hacked-between-apr-2017-jan-2018-118030700870\_1.html.

[^07NafisHasan_2]: For instance, see Shira Ovide, ‘A Fix-It Job for Government Tech’,
    24 November 2021,
    https://www.nytimes.com/2021/11/24/technology/government-tech.html.

[^07NafisHasan_3]: ‘Infosys Annual Report, 1993–94’, April 1994,
    https://www.infosys.com/investors/reports-filings/annual-report/annual/documents/infosys-ar-94.pdf.

[^07NafisHasan_4]: George Chacko, ‘INFOSYS: New Game, New Rules: A Case Study’,
    *Management Research News* 27.8/9 (2004): 1–25.

[^07NafisHasan_5]: ‘New System for Maruti Launched’, *The Times of India*, 25 October
    1994, sec. In Brief, ProQuest Historical Newspapers.

[^07NafisHasan_6]: ‘Pune Bourse Goes Online’, *The Times of India*, 19 March 1996,
    ProQuest Historical Newspapers.

[^07NafisHasan_7]: Martin Campbell-Kelly, ‘The RDBMS Industry: A Northern California
    Perspective’, *IEEE Annals of the History of Computing* 34.4 (2012):
    19.

[^07NafisHasan_8]: Paul Dourish, ‘No SQL: The Shifting Materialities of Database
    Technology’, *Computational Culture*, 4 November 2014, p. 2.

[^07NafisHasan_9]: Arun Mohan Sukumar, *Midnight’s Machines: A Political History of
    Technology in India*, New Delhi: Penguin Viking, 2019.

[^07NafisHasan_10]: Thomas Friedman, ‘‘Will India Seize the Moment?’’, *Seattle
    Post-Intelligencer*, 1924, 23 March 2004.

[^07NafisHasan_11]: [Miles
    Brignall](https://www.theguardian.com/profile/milesbrignall), ‘HSBC
    Indian Call Centre Worker Accused of Hacking into Accounts’, *The
    Guardian*, 29 June 2006,
    https://www.theguardian.com/money/2006/jun/29/business.india.

[^07NafisHasan_12]: Andrew Barry, Thomas Osborne and Nikolas Rose (eds), *Foucault
    and Political Reason: Liberalism, Neo-liberalism and Rationalities
    of Government*, Chicago: University of Chicago Press, 1996.

[^07NafisHasan_13]: Barry et al., *Foucault and Political Reason*, p. 12.

[^07NafisHasan_14]: This example has been drawn from my research for The Identity
    Project in 2011 and 2012, in which, among other things, I focused on
    the Aadhaar enrolments of Delhi’s homeless population. See Ashish
    Rajadhyaksha (ed), *In the Wake of Aadhaar: The Digital Ecosystem of
    Governance in India*, Bangalore: Centre for the Study of Culture and
    Society, 2013. Aadhaar is the Government of India’s biometric
    identity project for its billion plus residents.

[^07NafisHasan_15]: Atul Kohli, ‘Politics of Economic Growth in India, 1980–2005 Part
    II: The 1990s and Beyond’, *Economic & Political Weekly*, 41.13
    (2006): 1251–1259.

[^07NafisHasan_16]: I thank Christopher Kelty at UCLA for suggesting that layers of
    technological forms could be thought of as strata of a geological
    formation.

[^07NafisHasan_17]: Personal interview with the Director of NIC Shillong, Timothy
    Dkhar, in September 2019.

[^07NafisHasan_18]: Venkat Ananth, ‘Government of India: The World’s Biggest App
    Factory’, *The Ken*, 17 October 2016,
    https://the-ken.com/story/government-india-worlds-biggest-app-factory/.

[^07NafisHasan_19]: Ananth, ‘Government of India’.

[^07NafisHasan_20]: National Council of Applied Economic Research, *The NCAER Land
    Records and Services Index (N-LRSI) 2020*, Report 20200201, February
    2020, https://www.ncaer.org/publication\_details.php?pID=317.

[^07NafisHasan_21]: The National e-Governance Plan is an initiative of the Government
    of India to make all government services available to the citizens
    of India via electronic media. For details, see
    https://www.meity.gov.in/divisions/national-e-governance-plan.

[^07NafisHasan_22]: Personal interview with the Director of NIC Shillong, Timothy
    Dkhar, in September 2019.

[^07NafisHasan_23]: ‘Over 22k Indian Websites, 114 Govt Portals Hacked’.

[^07NafisHasan_24]: See ‘Chapter 6: Transfer of Personal Data Outside India’, in
   Committee of Experts under the
    Chairmanship of Justice B.N. Srikrishna, *A Free and Fair Digital
    Economy: Protecting Privacy, Empowering Indians*, Ministry of
    Electronics and Information Technology, Government of India, 2018,
    https://www.meity.gov.in/writereaddata/files/Data\_Protection\_Committee\_Report.pdf..
    Also see, Parminder Jeet Singh, ‘Bringing
    Data under the Rule of Law’, *The Hindu*, 20 September 2018,
    https://www.thehindu.com/opinion/op-ed/bringing-data-under-the-rule-of-law/article24988755.ece.

[^07NafisHasan_25]: Barry et al., *Foucault and Political Reason.*

[^07NafisHasan_26]: Aihwa Ong, *Neoliberalism as Exception:
    Mutations in Citizenship and Sovereignty*, Durham: Duke University
    Press, 2006, p. 6.

[^07NafisHasan_27]: Narasimhiah Seshagiri was a computer scientist under whose
    supervision the NIC was set up in the late 70s. Impressed by NIC’s
    ability to set up an Information Management System for the ninth
    Asian Games held in 1982 in Delhi, the then Prime Minister Rajiv
    Gandhi adopted Seshagiri’s policy on computers that set the stage
    for much of the e-governance to come. See Sukumar, *Midnight’s
    Machines*.

[^07NafisHasan_28]: Lilly Irani, *Chasing
    Innovation: Making Entrepreneurial Citizens in Modern India*,
    Princeton: Princeton University Press, 2019.

[^07NafisHasan_29]: Irani, *Chasing Innovation*, p. 7.

[^07NafisHasan_30]: ‘Computerized Data Bank’ - Consultancy Assistance from
    Institutions (1976), File No. M-12038/3/76 – M&I, National Archives
    of India.

[^07NafisHasan_31]: ‘Thick’ and ‘Thin’ is one of the many binaries in which forms of
    citizenship have come to be expressed, as recounted by Niraja Gopal
    Jayal, *Citizenship and its Discontents: An Indian History*,
    Cambridge, MA: Harvard University Press, 2013, p. 3.

[^07NafisHasan_32]: Planning Commission, ‘Standing
    Committee for Directing and Reviewing Improvement of Data Base for
    Planning and Policy Making’, Vol. I, 1978, File No.
    O-11-17/1/78-M&I, National Archives of India.

[^07NafisHasan_33]: Planning Commission, ‘Standing Committee for Directing and
    Reviewing Improvement of Data base for Planning and Policy Making’.

[^07NafisHasan_34]: Planning Commission, ‘Standing Committee for Directing and
    Reviewing Improvement of Data base for Planning and Policy Making’.

[^07NafisHasan_35]: J.G. Krishnayya et al. (eds), *sacm: A Monthly Magazine,* Pune:
    Systems Research Institute, 1979, p. 1.

[^07NafisHasan_36]: Krishnayya et al., *sacm,* p. 1.

[^07NafisHasan_37]: Krishnayya et al., *sacm*, p. 1.

[^07NafisHasan_38]: Krishnayya et al, *sacm*, p. 2.

[^07NafisHasan_39]: Unnamed File, File No. O-11717/5/75
    M&I, National Archives of India.

[^07NafisHasan_40]: Krishnayya et al, *sacm*, p. 2.

[^07NafisHasan_41]: Unnamed File, File No. O-11717/5/75 M&I, National Archives of
    India.

[^07NafisHasan_42]: Yojana Bhavan, which translates to Planning Office, is a physical
    building which housed India’s Planning Commission since its
    inception in March 1950.

[^07NafisHasan_43]: Planning Commission, ‘Setting up of a National Informatics Centre
    - Proposal from the Electronics Commission’, 1977, File No.
    11017/5/77 M&I, National Archives of India.

[^07NafisHasan_44]: The Electronics Commission has an interesting genesis as it was
    directly set up by M.G.K. Menon with the prime minister’s blessings.

[^07NafisHasan_45]: Unnamed File. File No. O-11717/5/75 M&I, National Archives of
    India.

[^07NafisHasan_46]: ‘Setting up of a National Informatics
    Centre - Proposal from the Electronics Commission’, File No.
    11017/5/77 M&I, National Archives of India.

[^07NafisHasan_47]: ‘Setting up of a National Informatics Centre’.

[^07NafisHasan_48]: Michael Castelle, ‘Relational and
    Non-Relational Models in the Entextualization of Bureaucracy’,
    *Computational Culture* 3 (November 2013).
    http://computationalculture.net/relational-and-non-relational-models-in-the-entextualization-of-bureaucracy/.

[^07NafisHasan_49]: This was between August and September 2019 at the NIC in
    Shillong.

[^07NafisHasan_50]: Castelle, ‘Relational and Non-Relational Models’.

[^07NafisHasan_51]: Castelle, ‘Relational and Non-Relational Models’.

[^07NafisHasan_52]: Castelle, ‘Relational and Non-Relational Models’.

[^07NafisHasan_53]: David Alan Grier, ‘The Relational
    Database and the Concept of the Information System', *IEEE Annals of
    the History of Computing* 34.4 (2012): 13.

[^07NafisHasan_54]: Dewang Mehta,
    ‘India on the Global Pathway’, *Times of India*, 7 February 1996,
    ProQuest Historical Newspapers.

[^07NafisHasan_55]: Campbell-Kelly, ‘The RDBMS Industry', p. 18.

[^07NafisHasan_56]: IDM-Informix Tie-up, *Times of
    India*, 24 December 1989, ProQuest Historical Newspapers.

[^07NafisHasan_57]: ‘IDM-Informix Tie-up’.

[^07NafisHasan_58]: Aprajita Sikri, ‘A US-Indian Database
    Venture’, *India Abroad*, 1 June 1990, ProQuest Historical
    Newspapers.

[^07NafisHasan_59]: Campbell-Kelly, ‘The RDBMS Industry', p. 21.

[^07NafisHasan_60]: Campbell-Kelly, ‘The RDBMS Industry', p. 22.

[^07NafisHasan_61]: ‘Oracle Opens India Liaison Office’,
    *Dataquest*, 1991,
    https://itihaasa.com/describe/artefact/001\_001\_0568?referenceYear=1991.

[^07NafisHasan_62]: ‘Oracle Opens India Liaison Office’.

[^07NafisHasan_63]: ‘Nalanda Computer Education for RDBMS’,
    *The* *Times of India*, 29 May 1991, ProQuest Historical Newspapers.

[^07NafisHasan_64]: ‘Overseas Appointments’, *The* *Times
    of India*, 20 September 1992, ProQuest Historical Newspapers;
    ‘Appointments,’ *The Times of India*, 6
    April 1993, ProQuest Historical Newspapers; []‘Tata Unisys Ltd’, *The* *Times of India*, 28 December 1993,
    ProQuest Historical Newspapers.

[^07NafisHasan_65]: ‘On the Move’, *The* *Times of India*,
    22 March 1993, ProQuest Historical Newspapers.

[^07NafisHasan_66]: Madhu Valluri, ‘How Info-tech can Help
    Environment’, *The Times of India*, 14 April 1993, ProQuest
    Historical Newspapers.

[^07NafisHasan_67]: Valluri, ‘How Info-tech can Help Environment’.

[^07NafisHasan_68]: ‘Pune Bourse Goes Online’.

[^07NafisHasan_69]: ‘4-Day Conference Opens’, *The* *Times
    of India*, 8 February 1996, ProQuest Historical Newspapers.

[^07NafisHasan_70]: Rajesh Y.P., ‘Software Firms Eye a Pie
    in Banking’, *News - India Times*, 10 July 1998, ProQuest Historical
    Newspapers

[^07NafisHasan_71]: Moneesh Narula, ‘Bank Automation Gets
    Competitive’, *The Times of India*, 4 September 1993, ProQuest
    Historical Documents.

[^07NafisHasan_72]: Narula, ‘Bank Automation Gets Competitive’.

[^07NafisHasan_73]: T. Narayanaswami, ‘The Central
    Solution’, *The Times of India*, 7 May 1996, ProQuest Historical
    Documents.

[^07NafisHasan_74]: In the words of the international authors presenting a case study
    of PRS transformation in Milwaukee, ‘RDBMS-based data management, in
    place of the older file-based data management sub-system was being
    used. A decade ago, RDBMSs had been expensive and
    resource-intensive, and the desired user response times had been
    difficult to obtain in large RDBMS-based applications. Nowadays,
    hardware resources were no longer a constraint, and the flexible
    data structures possible with an RDBMS core would greatly enhance
    overall application flexibility’. See []Shirish C. Srivastava, Sharat Mathur and Thompson Teo,
    ‘Modernization of Passenger Reservation System: Indian Railway’s
    Dilemma, *ICIS 2006 Proceedings* 98 (2006).
    http://aisel.aisnet.org/icis2006/98.

[^07NafisHasan_75]: Srivastava et al., ‘Modernization of Passenger Reservation
    System’, p. 434.

[^07NafisHasan_76]: Srivastava et al., ‘Modernization of Passenger Reservation
    System’, p. 437.

[^07NafisHasan_77]: R.S. Smith, ‘Rule-by-Records and
    Rule-by-Reports: Complementary Aspects of British Imperial Rule of
    Law’, *Contributions to Indian sociology* 19.1 (1985): 153–176.

[^07NafisHasan_78]: D.C. Wadhwa, ‘Guaranteeing Title to
    Land’, *Economic and Political Weekly* 37.47 (2002): 4704.

[^07NafisHasan_79]: Personal conversation with the cofounder of Comat Technologies,
    Ravi Ranjan, in August 2019 in Bangalore.

[^07NafisHasan_80]: Personal conversation with the director of NIC Kurukshetra in
    July 2018.

[^07NafisHasan_81]: At the India Land and Development Conference 2020, Tim Hanstead,
    the CEO of Landesa, pointed out that it was ironical that India
    leads the world in IT, but in the 20 years that the program on land
    modernization has seen, very little progress has been achieved.

[^07NafisHasan_82]: This was made apparent to me in conversations with the architect
    of the Bhoomi database in Bangalore, in August 2019.

[^07NafisHasan_83]: Akshatha M, ‘Land Sharks Hack Bhoomi
    Data, Shift Government Land Title’, *The Economic Times*, 10
    September 2018,
    https://economictimes.indiatimes.com/news/politics-and-nation/land-sharks-hack-bhoomi-data-shift-government-land-title/articleshow/65749538.cms.

[^07NafisHasan_84]: Bhoomi software, introduced to digitize land records, came into
    being in 2002.

[^07NafisHasan_85]: Akshatha, ‘Land Sharks Hack Bhoomi Data’.

[^07NafisHasan_86]: Elisa Bertino and Ravi Sandhu,
    ‘Database Security—Concepts, Approaches, and Challenges’, *IEEE
    Transactions on Dependable and Secure Computing* 2.1 (2005): 2.

[^07NafisHasan_87]: Michael Geertz and Madhavi Gandhi,
    ‘Security Re-engineering for Databases: Concepts and Techniques’, in
    Michael Geertz and Sushil Jajodia (eds) *Handbook of Database
    Security: Applications and Trends*, New York: Springer, 2008, pp.
    267–298.

[^07NafisHasan_88]: Geertz and Gandhi, ‘Security Re-engineering for Databases’.

[^07NafisHasan_89]: Harshavardhan Kayarkar, ‘Classification
    of Various Security Techniques in Databases and their Comparative
    Analysis’, *arXiv preprint arXiv* 1206.4124 (2012): 1 and Seul-Gi
    Choi and Sung-Bae Cho, ‘Evolutionary Reinforcement Learning for
    Adaptively Detecting Database Intrusions’, *Logic Journal of the
    IGPL* 28.4 (2020): 449–460.

[^07NafisHasan_90]: Y. Khmelevsky, ‘Information and Data
    Protection Within a RDBMS’, *Condensed Matter Physics* 11.4 (2008):
    761–765.

[^07NafisHasan_91]: Michael Geertz and Sushil Jajodia (eds)
    *Handbook of Database Security: Applications and Trends*, New York:
    Springer, 2008, p. v.

[^07NafisHasan_92]: Bertino and Sandhu, ‘Database Security, p. 2.

[^07NafisHasan_93]: ‘eDistrict Mission Mode Project Under
    the National eGovernance Plan. Pilot Implementation Guidelines’,
    Department of Information Technology, Government of India, January
    2009,
    https://www.meity.gov.in/writereaddata/files/eDistGuidelines\_Feb09(rev1).pdf.

[^07NafisHasan_94]: ‘eDistrict Mission Mode Project Under the National eGovernance
    Plan’.

[^07NafisHasan_95]: Amar Jeet Singh and Rajesh Chauhan, ‘E-Government Databases: A
    Retrospective Study’, Indian Journal of Computer Science and
    Engineering 1.2 (2010): 72.

[^07NafisHasan_96]: Singh and Chauhan, ‘E-Government Databases’, p. 71.

[^07NafisHasan_97]: Rob Nixon, *Slow Violence and the Environmentalism of the Poor*,
    Cambridge, MA: Harvard University Press, 2011.

[^07NafisHasan_98]: See Committee of Experts under the Chairmanship of Justice B.N.
    Srikrishna, *A Free and Fair Digital Economy*. Hereafter referred to
    as the Srikrishna report.

[^07NafisHasan_99]: Srikrishna report, p. 82.

[^07NafisHasan_100]: Benjamin Baez, *Technologies of Government: Politics and Power
    in the “Information Age”*, Charlotte, North Carolina: Information
    Age Publishing, 2014.

[^07NafisHasan_101]: Grier, ‘The Relational Database’, p. 16.

[^07NafisHasan_102]: Grier, ‘The Relational Database’, p. 16.

[^07NafisHasan_103]: ‘Setting up of a National Informatics Centre’.

[^07NafisHasan_104]: ‘Setting up of a National Informatics Centre’. Emphasis is mine.

[^07NafisHasan_105]: ‘Why Late Justice Krishna Iyer Opposed Biometric Aadhaar’,
    *ToxicsWatch*, 10 December 2014,
    http://www.toxicswatch.org/2014/12/why-late-justice-krishna-iyer-opposed.html.

[^07NafisHasan_106]: ‘Setting up of a National Informatics Centre’.

[^07NafisHasan_107]: ‘Setting up of a National Informatics Centre’.

[^07NafisHasan_108]: ‘Setting up of a National Informatics Centre’.

[^07NafisHasan_109]: ‘Setting up of a National Informatics Centre’, p. 19.

[^07NafisHasan_110]: ‘Setting up of a National Informatics Centre’, p. 21.

[^07NafisHasan_111]: ‘Setting up of a National Informatics Centre’, p. 21.

[^07NafisHasan_112]: ‘Request for Proposal (RFP) For
    Selection of SWAN TPA’,
    https://www.meity.gov.in/writereaddata/files/An8\_Indicative\_SWAN.pdf.

[^07NafisHasan_113]: ‘Request for Proposal (RFP) For Selection of SWAN TPA’, p. 8.

[^07NafisHasan_114]: ‘WGITA – IDI Handbook on IT Audit for
    Supreme Audit Institutions’, February 2014,
    https://icisa.cag.gov.in/resource\_files/c60986ef8dd5d4f658df077c1b5dceb7.PDF.

[^07NafisHasan_115]: ‘WGITA – IDI Handbook on IT Audit’, p. 1.

[^07NafisHasan_116]: ‘WGITA – IDI Handbook on IT Audit’, p. 39.

[^07NafisHasan_117]: ‘WGITA – IDI Handbook on IT Audit’, p. 90.

[^07NafisHasan_118]: ‘WGITA – IDI Handbook on IT Audit’, p. 90.

[^07NafisHasan_119]: Nils Gilman, Jesse Goldhammer and
    Steven Weber, ‘Can You Secure an Iron Cage?’, *Limn*, Issue 8,
    February 2017,
    https://limn.it/articles/can-you-secure-an-iron-cage/.
