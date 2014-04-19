17. The Future
 
 17.1. copyright
            THE  CYPHERNOMICON: Cypherpunks FAQ and More, Version 0.666,
            1994-09-10, Copyright Timothy C. May. All rights reserved.
            See the detailed disclaimer. Use short sections under "fair
            use" provisions, with appropriate credit, but don't put your
            name on my words.
 
 17.2. SUMMARY: The Future
   17.2.1. Main Points
           - where things are probably going
   17.2.2. Connections to Other Sections
   17.2.3. Where to Find Additional Information
   17.2.4. Miscellaneous Comments
 
 17.3. Progress Needed
   17.3.1. "Why have most of the things Cypherpunks talk about *not*
            happened?"
           + Except for remailers and basic crypto, few of the main
              ideas talked about for so long have actually seen any kind
              of realization. There are many reasons:
            A. Difficult to achieve. Both Karl Kleinpaste and Eric
                Hughes implemented simple first-generation remailers in a
                matter of _days_, but "digital cash" and "aptical
                foddering," for example, are not quite so
                straightforward. (I am of course not taking anything away
                from Kleinpaste, Hughes, Helsingius, Finney, etc., just
                noting that redirecting mail messages--and even
                implementing PGP and things like delay, batching, etc.,
                into remailers--is a lot easier conceptually than DC-Nets
                and the like.
            B. Protocols are confusing, tough to implement. Only a tiny
                fraction of the "crypto primitives" discussed at Crypto
                Conferences, or in the various crypto books, have been
                realized as runnable code. Building blocks like "bit
                commitment" have not even--to my knowledge--been
                adequately realized as reusable code. (Certainly various
                groups, such as Chaum's, have cobbled-together things
                like bit commitment....I just don't think there's a
                consensus as to the form, and this has limited the
                ability of nonspecialists to use these "objects.")
            C. Semantic confusion as well. While it's fairly clear what
                "encrypting" or "remailing" means, just what is a
                "digital bank"? Or a "reputation server"?
            D. Interoperablity is problematic. Many platforms, many
                operating systems, many languages. Again, remailers and
                encryption work because there is a de facto lowest common
                denominator for them: the simple text block, used in e-
                mail, editors, input and output from programs, etc. That
                is, we all mostly know exactly what an ASCII text block
                is, and crypto programs are expected to know how to
                access and manipulate such blocks. This largely explains
                the success of PGP across many platforms--text blocks are
                the basic element. Ditto for Cypherpunks remialers, which
                operate on the text blocks found in most mail systems.
                The situation becomes much murkier for things like
                digital money, which are not standalone objects and are
                often multi-party protocols involving time delays,
                offline processing, etc.
            E. Lack of an economic motive. We on this list are not being
                paid to develop anything, are not assisted by anyone, and
                don't have the financial backing of corporations to
                assist us. Since much of today's "software development"
                is actually _deal-making_ and _standards negotiation_, we
                are left out of lots of things.
 
 17.4. Future Directions
   17.4.1. "What are some future directions?"
   17.4.2. The Future of the List
           + "What can be done about these situations?"
             - That is, given that the Cypherpunks list often contains
                sensitive material (see above), and given that the
                current membership list can be accessed by..... what can
                be done?
             - Move central server to non-U.S. locale
             - Or to "cyberspace" (distributed network, with no central
                server...like FidoNet)
             - subscribers can use pseudonyms, cutouts, remailers
   17.4.3. What if encryption is outlawed?
           - can uuencode (and similar), to at least slow down the
              filter programs a bit (this is barely security through
              obscurity, but....)
           - underground movements?
           - will Cypherpunks be rounded up?
   17.4.4. "Should Cypherpunks be more organized, more like the CPSR,
            EFF, and EPIC?"
           - Those groups largely are lobbying groups, with a staff in
              Washington supported by the membership donations of
              thousands or tens of thousands of dues-paying members. They
              perform a valuable service, of course.
           - But that is not our model, nor can it plausibly be. We were
              formed as an ad hoc group to explore crypto, were dubbed
              "Cypherpunks," and have since acted as a techno-grasssroots
              anarchy. No staff, no dues, no elections, no official rules
              and regulations, and no leadership beyond what is provided
              by the power of speech (and a slight amount of "final say"
              provided by the list maintainer Eric Hughes and the machine
              owner, John Gilmore, with support from Hugh Daniel).
           - If folks want a lobbying group, with lawyers in Washington,
              they should join the EFF and/or CPSR.
           - And we fill a niche they don't try to fill.
   17.4.5. Difficult to Set Directions
           - an anarchy...no centralized control
           - emergent interests
           - everyone has some axe to grind, some temporary set of
              priorities
           - little economic motivation (and most have other jobs)
   17.4.6. The Heart and Soul of Cypherpunks?
           + Competing Goals:
             + Personal Privacy
               - PGP, integration with mailers
               - education
             + Reducing the Power of Institutions
               - whistelblowers group
               -
             - Crypto Anarchy
           + Common Purposes
             + Spreading strong crypto tools and knowledge
               - PGP
             + Fighting government restrictions and regulations
               - Clipper/Skipjack fight was a unifying experience
             + Exploring new directions in cryptology
               - digital mixes, digital cash, voting
   17.4.7. Possible Directions
           + Crypto Tools...make them ubiquitous "enough" so that the
              genie cannot be put back in the bottle
             - can worry about the politics later (socialists vs.
                anarchocapitalists, etc.) (Although socialists would do
                well to carefully think about the implications of
                untraceable communications, digital cash, and world-wide
                networks of consultants and workers--and what this does
                to tax collection and social spending programs--before
                they work with the libertarians and anarchocapitalists to
                bring on the Crypto Millenium.)
           + Education
             - educating the masses about crypto
             - public forums
             - this was picked by the Cambridge/MIT group as their
                special interest
           + Lobbying
             - talking to Congressional aides and committee staffers,
                attending hearings, submitting briefs on proposed
                legislation
             - coordinating with EFF, CPSR, ACLU, etc.
             - this was picked by the Washington group as their special
                interest, which is compellingly appropriate (Calif. group
                is simply too far away)
           - Legal Challenges
           + mixture of legal and illegal
             - use legal tools, and illegal tools
             - fallback positions
             - enlist illegal users as customers...help it spread in
                these channels (shown to be almost uncontrollable)
   17.4.8. Goals (as I see them)
           + Get strong crypto deployed in such a way as to be
              unstoppable, unrecallable
             - "fire and forget" crypto
             - genie out of the bottle
             - Note that this does _not_ necessarily that crypto be
                _widely_ deployed, though that's generally a good idea.
                It may mean seeding key sites outside the U.S. with
                strong crypto tools, with remailers, and with the other
                acouterments.
           + Monkeywrench threats to crypto freedom.
             - economic sabotage of those who use statist contracts to
                thwart freedom (e.g., parts of AT&T)
             + direct sabotage
               - someday, viruses, HERF, etc.
   17.4.9. A Vision of the Future
           - encrypted, secure, untraceable communications
           - hundreds of remailers, in many countries
           - interwoven with ordinary traffic, ensuring that any attempt
              to quash crypto would also have a dramatic effect on
              business
           - data havens, credit, renters, etc.
           - information markets
           - ability to fight wars is hindered
           - U.S. is frantic, as its grip on the world loosens...Pax
              Americana dies
  17.4.10. Key concepts are the way to handle the complexity of crypto
           - The morass of protocols, systems, and results is best
              analyzed, I think, by not losing sight of the basic
              "primitives," the things about identity, security,
              authentication, etc. that make crypto systems work the way
              they do.
           + Axiom systems, with theorems and lemmas derivable from the
              axioms
             - with alternate axioms giving the equivalent of "non-
                Euclidean geometries" (in a sense, removing the physical
                identity postulate and replacing it with the "the key is
                the identity" postulate gives a new landscape of
                interactions, implications, and structures).
           - (Markets, local references, voluntary transactions, etc.)
           - (ecologies, predators, defenders, etc.)
           - (game theory, economics, etc..)
 
 17.5. Net of the Future
   17.5.1. "What role, if any, will MUDs, MOOs, and Virtual Realities
            play?"
           - "True Names," "Snow Crash," "Shockwave Rider"
           - Habitat, online services
           + the interaction is far beyond just the canonical "text
              messages" that systems like Digital Telephony are designed
              to cope with
             - where is the nexus of the message?
             - what about conferences scattered around the world, in
                multiple jurisdictions?
           - crypto = glue, mortar, building blocks
           - "rooms" = private places; issues of access control
           - Unless cops are put into these various "rooms," via a
              technology we can barely imagine today (agents?), it will
              be essentially impossible to control what happens in these
              rooms and places. Too many degrees of freedom, too many
              avenues for exchange.
           - cyberspaces, MUDs, virtual communities, private law,
              untouchable by physical governments
   17.5.2. keyword-based
           - can be spoofed by including dictionaries
   17.5.3. dig sig based (reputation-based)
   17.5.4. pools and anonymous areas may be explicitly supported
   17.5.5. better newsreaders, screens, filters
   17.5.6. Switches
           - "switching fabrics"
           - ATM
           - Intel's flexible mesh interconnects, iWARP, etc.
           - all of these will make for an exponential increase in
              degrees of freedom for remailer networks (labyrinths). On-
              chip remailing is esentially what is needed for Chaum's
              mixes. ATM quanta (packets) are the next likely target for
              remailers.
   17.5.7. "What limits on the Net are being proposed?"
           - NII
           + Holding carriers liable for content
             - e.g., suing Compuserve or Netcom
             - often done with bulletin boards
           - "We have to do something!"
           + Newspapers are complaining about the Four Horsemen of the
              Infocalypse:
             - terrorists, pedophiles, drug dealers, and money
                launderers
             + The "L.A. Times" opines:
               - "Designers of the new Information Age were inspired by
                  noble dreams of free-flowing data as a global
                  liberating force, a true democratizing agent.  Sadly,
                  the crooks and creeps have also climbed aboard.  The
                  time has come for much tighter computer security.
                  After all, banks learned to put locks on their vaults."
                  ["L.A. Times," editorial, 1994-07-13]
 
 17.6. The Effects of Strong Crypto on Society
   17.6.1. "What will be the effects of strong crypto, ultimately, on
            the social fabric?"
           - It's hard to know for sure.
           + These effects seem likely:
             - Starvation of government tax revenues, with concommitant
                effects on welfare, spending, etc.
             - increases in espioage
             - trust issues
   17.6.2. The revelations of surveillance and monitoring of citizens
            and corporations will serve to increase the use of
            encryption, at first by people with something to hide, and
            then by others. Cypherpunks are already helping by spreading
            the word of these situations.
           - a snowballing effect
           - and various government agencies will themselves use
              encryption to protect their files and their privacy
   17.6.3. People making individual moral choices
           - people will make their own choices as to what to reveal,
              what they think will help world peace, or the future, or
              the dolphins, or whatever
           - and this will be a liquid market, not just souls shouting
              in the desert
           - of course, not everything will be revealed, but the "mosaic
              effect" ensures that mostly the truth will emerge
           - every government's worst fear, that it's subjects will
              decide for themselves what is secret, what is not, what can
              be told to foreigners, etc.
 
 17.7. New Software Tools and Programming Frameworks
   17.7.1. Needed software
           - Drop-in crypto modules are a needed development. As V.
              Bontchev says, "it would be nice if disk encryption
              software allowed the user to plug in their own modules.
              This way everybody could use whatever they trust - MDC/SHA,
              MDC/MD5, DES, IDEA, whatever." [V.B., sci.crypt, 1994-07-
              01]
           + Robustness
             - Security and robustness are often at odds
             - Files that are wiped at the first hint of intrusion
                (digital flash paper), remailer sites that go down at the
                first signs of trouble, and file transmission systems
                that split files into multiple pieces--any one of which
                can be lost, thus destroying the whole transmission--are
                not exactly models of robustness.
             - Error correction usually works by decreasing entropy
                through redundancy, which is bad for crypto.
             - The military uses elaborate (and expensive) systems to
                ensure that systems do not go down, keys are not lost,
                etc. Most casual users of crypto are unwilling to take
                these steps.
             - And so keys are lost, passphrases are forgotten (or are
                written down on Post-It Notes and taped to terminals),
                and remailers are taken down when operators go on
                vacation. All very flaky and non-robust.
             - Look at how flaky mail delivery is!
             + A challenge is to create systems which are:
               - robust
               - not too complicated and labor-intensive to use
               - where redundancy does not compromise security
           + Crypto workbench
             - An overused term, perhaps, but one that captures the
                metaphor of a large set of tools, templates, programming
                aids, etc.
             + QKS and "Agents Construction Kit" (under development)
               - along with Dylan, DylanAgents, Telescript, and probably
                  several other attempts to develop agent toolkits
             - Henry Strickland is using "tcl" (sort of a scripting
                language, like "perl") as a basis.
           + Software crisis
             - tools, languages, frameworks, environments, objects,
                class libraries, methods, agents, correctness,
                robustness, evolution, prototyping
             + Connections between the software crisis and cryptography
               - complex systems, complicated protocols
               - price of being "wrong" can be very high, whether it's
                  an airport that can't open on time (Denver) or a
                  digital bank that has its assets drained in seconds
               - agents, objects are hoped to be the "silver bullets"
             + The need for better software methodologies
               - "silver bullets"
               - failures, errors, flaws, methods
               - provably correct designs? (a la Viper)
               - It is often said that much better methodologies are
                  needed for _real time programming_, due to the time-
                  criticality and (probably) the difficulty of doing
                  realistic testing. But surely the same should be said
                  of _financial programming_, a la the banking and
                  digicash schemes that interest us so much.
               - "the one aspect of software that most makes it the
                  flaky industry it is is that it is unusual for
                  practitioners to study the work of others.  Programmers
                  don't read great programs.  Designers don't study
                  outstanding designs. The consequences ... no, just look
                  for yourself. [Cameron Laird, comp.software-eng, 1994-
                  08-30]
             + Large Software Constructs
               - The software crisis becomes particularly acute when
                  large systems are built, such as--to apply this to
                  Cypherpunks issues--when digital money systems and
                  economies are built.
   17.7.2. Object-oriented tools
           + While tres trendy, some very real gains are being reported;
              more than just a buzzword, especially when combined with
              other tools:
             - frameworks, toolkits
             + dynamic languages
               - greater flexibility than with static, strongly-typed
                  langueages (but also less safety, usually)
           - OpenStep, Visual Age, Visual Basic, Dylan, Telescript (more
              agent-oriented), Lisp, Smalltalk, etc
   17.7.3. Protocol Ecologies
           - Behavioral simulations of agents, digital money, spoofing,
              etc.
           - the world in which Alice and Bob and their crypto friends
              live
           - defense, attack, spoofing, impersonation, theft
           - elements that are cryptographically strong (like D-H key
              exchanges), but combined in complex ways that almost have
              to be simulated to find weaknesses
           - "middle-out" instead of "top-down" (conventional, formal)
              or "bottom-up" (emergent, A-LIFE)
           - like Eurisko (Lenat), except oriented toward the domain of
              financial agents
   17.7.4. Use of autonomous agents (slaves?)
           - "An advanced telecommunications environment offers a number
              of ways to protect yourself against the problems involved
              in dealing with anonymous entities in a situation in which
              there is no monopoly Government.....When one's PBX finds
              that one's call is not going through via a particular long
              distance carrier, it automatically switches to another one.
              It is easy to imagine one's intelligent agents testing
              various sorts of transaction completions and switching
              vendors when one fails. Professional checkers can supply
              information on vendor status for a fee. After all, we don't
              care if a company we are dealing with changes if its
              service is unaffected."  [Duncan Frissell, 1994-08-30]
   17.7.5. Tools
           + "Languages within languages" is a standard way to go to
              implement abstractions
             - "Intermediate Design Languages" (IDLs)
             - abstract concepts: such as "engines" and "futures"
             - Lisp and Scheme have been favored languages for this
             - other languages as well: Smalltalk, Dylan
           + For crypto, this seems to be the case: abstractions
              represented as classes or objects
             - with programming then the selective subclassing
             - and sometimes gener
           + "type checking" of crypto objects is needed
             - to ensure compliance with protocols, with forms expected,
                etc.
             - check messages for form, removal of sigs, etc. (analogous
                to checking a letter before mailing for proper
                addressing, for stamp, sealing, etc.)
             - much of the nonrobustness of mail and crypto comes from
                the problems with exception handling--things that a human
                involved might be able to resolve, in conventional mail
                systems
             - "dead letter department"?
             - Note: In the "Crypto Anarchy Game" we played in
                September, 1992, many sealed messages were discarded for
                being in the wrong form, lacking the remailer fee that
                the remailer required, etc. Granted, human beings make
                fairly poor maintainers of complex constraints....a lot
                of people just kept forgetting to do what was needed. A
                great time was had by all.
   17.7.6. "What programming framework features are needed?"
           - What follows are definitely my opnions, even more my own
              opinions than most of what I've written. Many people will
              disagree.
           + Needed:
             - Flexibility over speed
             - Rapid prototyping, to add new features
             - Evolutionary approaches
             - Robustness (provably correct would be nice, but...)
   17.7.7. Frameworks, Tools, Capabilities
           - Nearly all the cutting-edge work in operating systems, from
              "mutually suspicious cooperating processes" to "deadlock"
              to "persistence," show up in the crypto areas we are
              considering.
           + Software of the Net vs. Software to Access the Net
             - The Net--is current form adequate?
             - Software for Accessing the Net
           + OpenDoc and OLE
             - components working together, on top of various operating
                systems, on top of various hardware platforms
           + Persistent Object Stores
             - likely to be needed for the systems we envision
             - robust, so that one's "money" doesn't evaporate when a
                system is rebooted!
             - interesting issues here...
             - CORBA. OpenDoc, OLE II, SOM, DOE, Gemstone, etc.
           + Programming Frameworks
             - Dynamic languages may be very useful when details are
                fuzzy, when the ideas need exploration (this is not a
                call for nondeterminism, for random futzing around, but a
                recognition that the precise, strongly-typed approach of
                some languages may be less useful than a rich,
                exploratory environment. This fits with the "ecology"
                point of view.
             -
           + Connectivity
             - needs to be more robust, not flaky the way current e-mail
                is
             - handshakes, agents, robust connections
             - ATM, SONET, agents, etc....the "Net of the Future"
 
 17.8. Complexity
   17.8.1. The shifting sands of modern, complex systems
           - lots of cruft, detail...changing..related to the "software
              crisis"...the very flexibilty of modern software systems
              promotes the frequent changing of features and behaviors,
              thus playing hob with attempts of others to understand the
              structure...evolution in action
           - humans who use these systems forget how the commands work,
              where things are stored, how to unsubscribe from lists,
              etc. (This is just one reason the various sub-lists of our
              list have seldom gotten much traffic: people use what they
              are most used to using, and forget the rest.)
           - computer agents (scripts, programs) which use these systems
              often "break" when the underlying system changes. A good
              example of this are the remailer sites, and scripts to use
              them. As remailer sites go up and down, as keys change, as
              other things change, the scripts must change to keep pace.
           - This very document is another example. Scattered throughout
              are references to sites, programs, sources, etc. As time
              goes by, more and more of them will (inevitably) become
              obsolete. (My hope is that enough of the pointers will
              point to still-extant things so as to make the pointers
              remain useful. And I'll try to update/correct the bad
              pointers.)
   17.8.2. "Out of Control"
           - Kevin Kelly's book
           - inability to have precise control, and how this is
              consistent with evolution, emergent properties, limits of
              formal models
           - crypto, degrees of freedom
           + imagine nets of the near future
             - ten-fold increase in sites, users, domains
             - ATM switching fabrics..granularity of transactions
                changes...convergence of computing and communications...
             + distributed computation ( which, by the way, surely needs
                crypto security!)
               - Joule, Digital Silk Road
             - agents, etc.
           + can't control the distribution of information
             + As with the Amateur Action BBS case, access can't be
                controlled.
               - "The existance of gateways and proxy servers means that
                  there is no effective way to determine where any
                  information you make accessible will eventually end up.
                  Somebody in, say, Tennessee can easily get at an FTP
                  site in California through a proxy in Switzerland.
                  Even detailed information about what kind of
                  information is considered contraband in every
                  jurisdiction in the world won't help, unless every
                  *gateway* in the world has it and uses it as well."
                  [Stephen R. Savitzky, comp.org.eff.talk, 1994-08-08]
   17.8.3. A fertile union of cryptology, game theory, economics, and
            ecology
           + crypto has long ignored economics, except peripherally, as
              an engineering issue (how long encryption takes, etc.)
             - in particular, areas of reputation, risk, etc. have not
                been treated as central idea...perhaps proper for
                mathematical algorithm work
             - but economics is clearly central to the systems being
                planned...digital cash, data havens, remailers, etc.
           + why cash works so well...locality of reference, immediate
              clearing of transactions, forces computations down to
              relevant units
             - reduces complaints, "he made me do it" arguments...that
                is, increases self-responsibility...caveat emptor
           + game theory
             + ripe for treatment of "Alice and Bob" sorts of
                situations, in which agents with different agendas are
                interacting and competing
               - "defecting" as in Prisoner's Dilemma
               - payoff matrices for various behaviors
           - evolutionary game theory
           - evolutionary learning, genetic algorithms/programmming
           - protocol ecologies
 
 17.9. Crypto Standards
   17.9.1. The importance of standards
           - a critical role
           + Part of standards is validation, test suites, etc.
             - validating the features and security of a remailer,
                through pings, tests, performance tests, reliability,
                etc.
             - thus imposing a negative hit on those who fail
             + There are many ways to do this standards testing
               - market reports (as with commercial chips, software)
               - "seals of approval" (especially convenient with digital
                  sigs)

17.10. Crypto Research
  17.10.1. Academic research continues to increase
  17.10.2. "What's the future of crypto?"
           - Predicting the future is notoriously difficult. IBM didn't
              think many computers would ever be sold, Western Union
              passed on the chance to buy Bell's telephone patents. And
              so on. The future is always cloudy, the past is always
              clear and obvious.
           - We'll know in 30 years which of our cypherpunkish and
              cryptoanarchist predictions came to pass--and which didn't.
  17.10.3. Ciphers are somewhat like knots...the right sequence of moves
            unties them, the wrong sequence only makes them more tangled.
            ("Knot theory" is becoming a hot topic in math and physics
            (work of Vaughn Jones, string theory, etc.) and I suspect
            there are some links between knot theory and crypto.)
  17.10.4. Game theory, reputations, crypto -- a lot to be done here
           - a missing link, an area not covered in academic cryptology
              research
           - distributed trust models, collusion, cooperation,
              evolutionary game theory, ecologies, systems
  17.10.5. More advanced areas, newer approaches
           + some have suggested quasigroups, Latin squares, finite
              automata, etc. Quasigroups are important in the IDEA
              cipher, and in some DES work. (I won't speculate furher
              about an area I no almost nothing about....I'd heard of
              semigroups, but not quasigroups.)
             - "The "Block Mixing Transform" technology which I have
                been promoting on sci.crypt for much of this spring and
                summer is a Latin square technology.  (This was part of
                my "Large Block DES" project, which eventually produced
                the "Fenced DES" cipher as a possible DES
                upgrade.)....Each of the equations in a Block Mixing
                Transform is the equation for a Latin square.  The
                multiple equations in such a transform together represent
                orthogonal Latin squares. [Terry Ritter, sci.crypt, 1994-
                08-15]
           + But what about for public key uses? Here's something Perry
              Metzger ran across:
             - ""Finte Automata, Latin arrays, and Cryptography" by Tao
                Renji, Institute of Software, Academia Sinica, Beijing.
                This (as yet unpublished) paper covers several
                fascinating topics, including some very fast public key
                methods -- unfortunately in too little detail. Hopefully
                a published version will appear soon..." [P.M.,
                sci.crypt, 1994-08-14]
  17.10.6. Comments on crypto state of the art today vs. what is likely
            to be coming
           - Perry Metzger comments on today's practical difficulties:
              "...can the difference between "crypto can be transforming
              when the technology matures" and "crypto is mature now" be
              that unobvious?....One of the reasons I'm involved with the
              IETF IPSP effort is because the crypto stuff has to be
              transparent and ubiquitous before it is going to be truly
              useful -- in its current form its just junk. Hopefully,
              later versions of PGP will also interface well with the new
              standards being developed for an integrated secure message
              body type in MIME. (PGP also requires some sort of scalable
              and reverse mapable keyid system -- the current keyids are
              not going to allow key servers to scale in a distributed
              manner.) Yes, I've seen the shell scripts and the rest, and
              they really require too much effort for most people -- and
              at best, once you have things set up, you can now securely
              read some email at some sites. I know that for myself,
              given that I read a large fraction of my mail while working
              at clients, where I emphatically do not trust the hardware,
              every encrypted message means great inconvenience,
              regardless." [Perry Metzger, 1994-08-25]

17.11. Crypto Armageddon? Cryptageddon?
  17.11.1. "Will there be a "Waco in cyberspace"?"
           - while some of us are very vocal here, and are probably
              known to the authorities, this is not generally the case.
              Many of the users of strong crypto will be discreet and
              will not give outward appearances of being code-using
              crypto anarchist cultists.
  17.11.2. Attacks to come
           - "You'll see these folks attacking anonymous remailers,
              cryptography, psuedonymous accounts, and other tools  of
              coercion-free expression and information  interchange on
              the net, ironically often in the name of promoting
              "commerce".  You'll hear them rant and rave about
              "criminals" and "terrorists", as if they even had a good
              clue about the laws of the thousands  of jurisdictions
              criss-crossed by the Internet, and as if their own attempts
              to enable coercion bear no resemblance to the practice of
              terrorism.  The scary thing is, they  really think they
              have a good idea about what all those laws should be, and
              they're perfectly willing to shove it down our throats,
              regardless of the vast diversity of culture, intellectual,
              political, and legal opinion on the planet."
              [<an50@desert.hacktic.nl> (Nobody),  libtech-l@netcom.com,
              1994-06-08]
           + why I'm not sanguine about Feds
             - killing Randy Weaver's wife and son from a distance,
                after trumped-up weapons charges
             - burning alive the Koresh compound, on trumped-up charges
                of Satanism, child abuse, and wife-insulting
             - seizures of boats, cars, etc., on "suspicion" of
                involvement with drugs

17.12. "The Future's So Bright, I Gotta Wear Shades"
  17.12.1. Despite the occasionally gloomy predictions, things look
            pretty good.No guarantees, of course, but trends that are
            favorable. No reason for us to rest, though.
  17.12.2. Duncan Frissell puts it this way:
           - "Trade is way up.  Wealth is way up.  International travel
              is way up. Migration is way up.  Resource prices are the
              lowest in human history.  Communications costs are way
              down.  Electronics costs are way down.  We are in a zero or
              negative inflation environment.  The quantity and quality
              of  goods and services offered on the markets is at an all-
              time high.  The percentage of the world's countries headed
              by dictators is the lowest it's ever been.
              
              "What all this means is that political philosophies that
              depend on force of arms to push people into line,  will
              increasingly fail to work.  Rich people with choices will,
              when  coerced, tend to change their investments and
              business affairs into a friendlier form or to move to a
              friendlier  environment.  Choice is real.  If choices
              exist, they will be made.  An ever higher proportion of the
              world's people will be "rich" in wealth and choice as the
              years go on.
              
              "Only a political philosophy that depends on the uncoerced
              cooperation of very  different people has a chance of
              functioning in  the future." [Duncan Frissell, 1994-09-09]

17.13. "Will cryptography really bring on the Millenium?"
  17.13.1. Yes. And cats will move in with dogs,  Snapple will rain from
            the sky, and P will be shown unequal to NP.
  17.13.2. Seriously, the implications of strong privacy, of
            cyberspatial economies, and of borders becoming transparent
            are enormous. The way governments do business is already
            changing, and this will change things even more dramatically.
            The precise form may be unpredictable, but certain end states
            are fairly easy to predict in broad brush strokes.
  17.13.3. "How do we know the implications of crypto are what I've
            claimed?"
           - We can't know the future.
           - Printing, railroads, electrification
  17.13.4. "When will it all happen? When will strong crypto really
            begin to have a major effect on the economy?"
           + Stages:
             - The Prehistoric Era. Prior to 1975. NSA and other
                intelligence agencies controlled most crypto work.
                Cryptography seen as a hobby. DES just starting to be
                deployed by banks and financial institutions.
             - The Research Era. 1975-1992. Intense interest in public
                key discovery, in various protocols. Start of several
                "Crypto" conferences. Work on digital money, DC-Nets,
                timestamping, etc.
             - The Activism Era. 1992--?? (probably 1998). PGP 2.0
                released. Cypherpunks formed. Clipper announced--meets
                firestorm of protest. EFF, CPSR, EPIC, other groups.
                "Wired" starts publication. Digital Telelphony, other
                bills. Several attempts to start crypto businesses are
                made...most founder.
             - The Transition Era. After about 1999. Businesses start.
                Digital cash needed for Net transactions. Networks and
                computers fast enough to allow more robust protocols. Tax
                havens flourish. "New Underworld Order" (credit to Claire
                Sterling) flourishes.
           - It is premature to expect that the current environment--
              technological and regulatory--will be beneficial to the
              type of strong crypto we favor. Too many pieces are
              missing. Several more advances are needed. A few more
              failures are also needed (gulp!) to show better how not to
              proceed.
  17.13.5. "But will crypto anarchy actually happen?"
           - To a growing extent, it already is happening. Look at the
              so-called illegal markets, the flows of drug money around
              the world, the transfer of billions of dollars a day on
              mere "chop marks," and the thriving trade in banned items.
           - "Grey and black capitalism is already a major component of
              international cash flows....Once adequate user friendly
              software is available, the internet will accellerate this
              already existing trend....Crypto anarchy is merely the
              application of modern tools to assist covert capitalism."
              [James Donald, 1994-08-29]
           - There are arguments that a Great Crackdown is coming, that
              governments will shut down illegal markets, will stop
              strong crypto, will force underground economies
              aboveground. This is doubtful--it's been tried for the past
              several decades (or more). Prohibition merely made crime
              more organized; ditto for the War on (Some) Drugs.
  17.13.6. "Has the point of no return been passed on strong crypto?"
           - Actually, I think that in the U.S. at least, the point was
              passed decades ago, possibly a century or more ago, and
              that any hope of controlling strong crypto and private
              communication evaporated long ago. Abuses by the FBI in
              wiretapping Americans, and reports of NSA monitoring of
              domestic communications notwithstanding, it is
              essentially.....

17.14. Loose Ends
  17.14.1. firewalls, virtual perimeters, swIPe-type encrypted tunnels,
            an end to break-ins,
  17.14.2. "What kind of encryption will be used with ATM?"
           - (ATM = Asynchronous Transfer Mode, not Automated Teller
              Machine)
           - some reports that NSA is developing standards for ATM
  17.14.3. Shapes of things to come, maybe....(laws of other countries)
           + India has a fee schedule for BBS operators, e.g., they have
              to pay $50,000 a year to operate a bulletin board! (This
              sounds like the urban legend about the FCC planning a modem
              tax, but maybe it's true.)
             - "The Forum for Rights to Electronic Expression (FREE) has
                been formed in India as a body dedicated to extending
                fundamental rights to the electronic domain....FREE owes
                its creation to an attack on Indian datacom by the Indian
                government, in the form of exorbitant licence fees (a
                minimum Rs. 1.5 million = US$50,000 each year for a BBS,
                much higher for e-mail)." [amehta@doe.ernet.in (Dr. Arun
                Mehta), forwarded by Phil Agre, comp.org.cpsr.talk, 1994-
                08-31]
             - for more info: ftp.eff.org
                /pub/EFF/Policy/World/India/FREE
  17.14.4. Cyberspace will need better protection
           - to ensure spoofing and counterfeiting is reduced (recall
              Habitat's problems with people figuring out the loopholes)
