12. Digital Cash and Net Commerce
 
 12.1. copyright
            THE  CYPHERNOMICON: Cypherpunks FAQ and More, Version 0.666,
            1994-09-10, Copyright Timothy C. May. All rights reserved.
            See the detailed disclaimer. Use short sections under "fair
            use" provisions, with appropriate credit, but don't put your
            name on my words.
 
 12.2. SUMMARY: Digital Cash and Net Commerce
   12.2.1. Main Points
           - strong crypto makes certain forms of digital cash possible
           - David Chaum is, once again, centrally involved
           - no real systems deployed, only small experiments
           - the legal and regulatory tangle will likely affect
              deployment in major ways (making a "launch" of digital cash
              a notrivial matter)
   12.2.2. Connections to Other Sections
           - reputations
           - legal situation
           - crypto anarchy
   12.2.3. Where to Find Additional Information
           - http://digicash.support.nl/
   12.2.4. Miscellaneous Comments
           - a huge area, filled with special terms
           - many financial instruments
           - the theory of digital cash is not complete, and confusion
              abounds
           - this section is also more jumbled and confusing than I'd
              like; I'll clean it up in fufure releases.
 
 12.3. The Nature of Money
   12.3.1. The nature of money, of banking and finance, is a topic that
            suffuses most discussions of digital cash. Hardly surprising.
            But also an area that is even more detailed than is crypto.
            And endless confusion of terms, semantic quibblings on the
            list, and so on. I won't be devoting much space to trying to
            explain economics, banking, and the deep nature or money.
   12.3.2. There are of course many forms of cash or money today (these
            terms are not equivalent...)
           + coins, bills (presumed to be difficult to forge)
             - "ontological conservation laws"--the money can't be in
                two places at once, can't be double spent
             - this is only partly true, and forgery technology is
                making it all moot
           - bearer bonds and other "immediately cashable" instruments
           - diamonds, gold, works of art, etc. ("portable wealth")
   12.3.3. Many forms of digital money. Just as there are dozens of
            major forms of instruments, so too will there be many forms
            of digital money. Niches will be filled.
   12.3.4. The deep nature of money is unclear to me. There are days
            when I think it's just a giant con game, with value in money
            only because others will accept it. Other days when I think
            it's somewhat tied to "real things" like gold and silver. And
            other days when I'm just unconcerned (so long as I have it,
            and it works).
   12.3.5. The digital cash discussions get similarly confused by the
            various ideas about money. Digital cash is not necessarily a
            form of _currency_, but is instead a transfer mechanism. More
            like a "digital check," in fact (though it may give rise to
            new currencies, or to wider use of some existing
            currency...at some point, it may become indistinguishable
            from a currency).
   12.3.6. I advise that people not worry overly much about the true and
            deep nature of money, and instead think about digital cash as
            a transfer protocol for some underlyng form of money, which
            might be gold coins, or Swiss francs, or chickens, or even
            giant stone wheels.
   12.3.7. Principle vs. Properties of Money
           - Physical coins, as money, have certain basic properties:
              difficult to counterfeit, pointless to counterfeit if made
              of gold or silver, fungibility, immediate settling (no need
              to clear with a distant bank, no delays, etc.),
              untraceability, etc.
           - Digital cash, in various flavors, has dramatically
              different properties, e.g., it may require clearing, any
              single digtital note is infinitely copyable, it may allow
              traceability, etc. A complicated mix of properties.
           + But why is physical money (specie) the way it is? What
              properties account for this? What are the core principles
              that imply these properties?
             - hardware (specie like gold) vs. software (bits, readily
                copyable)
             - immediale, local clearing, because of rational faith that
                the money will clear
             - limits on rate of transfer of physical money set by size,
                weight of money, whereas "wire fraud" and variants can
                drain an account in seconds
           - My notion is that we spend too much time thinking about the
              _principles_ (such as locality, transitivity, etc.) and
              expect to then _derive_ the properties. Maybe we need to
              instead focus on the _objects_, the sets of protocol-
              derived things, and examine their emergent properties. (I
              have my own thinking along these lines, involving "protocol
              ecologies" in which agents bang against each other, a la
              Doug Lenat's old "Eurisko" system, and thus discover
              weaknesses, points of strength, and even are genetically
              programmed to add new methods which increase security.
              This, as you can guess, is a longterm, speculative
              project.)
   12.3.8. "Can a "digital coin" be made?"
           - The answer appears to be "no"
           + Software is infinitely copyable, which means a software
              representation of digital money could be replicated many
              times
             - this is not to say it could be _spent_ many times,
                depending on the clearing process...but then this is not
                a "coin" in the sense we mean
           - Software is trivially replicable, unlike gold or silver
              coins, or even paper currency. If and when paper currency
              becomes trivially replicable (and color copiers have almost
              gotten there), expect changes in the nature of cash.
              (Speculation: cash will be replaced by smart cards,
              probably not of the anonymous sort we favor.)
           + bits can always be duplicated (unless tied to hardware, as
              with TRMs), so must look elsewhere
             + could tie the bits to a specific location, so that
                duplication would be obvious or useless
               - the idea is vaguely that an agent could be placed in
                  some location...duplications would be both detectable
                  and irrelevant (same bits, same behavior, unmodifiable
                  because of digital signature)
           - (this is formally similar to the idea of an active agent
              that is unforgeable, in the sense that the agent or coin is
              "standalone")
   12.3.9. "What is the 'granularity' of digital cash?"
           + fine granularity, e.g., sub-cent amounts
             - useful for many online transactions
             - inside computers
             - add-on fees by interemediaries
             - very small purchases
           + medium granularity
             - a few cents, up to a dollar (for example)
             - also useful for many small purchases
             - close equivalent to "loose change" or small bills, and
                probably useful for the same purposes
             - tolls, fees, etc.
             - This is roughly the level many DigiCash protocols are
                aimed at
           + large granularity
             - multiple dollars
             - more like a "conventional" online transaction
             -
           - the transaction costs are crucial; online vs. offline
              clearing
           - Digital Silk Road is a proposal by Dean Tribble and Norm
              Hardy to reduce transaction costs
  12.3.10. Debate about money and finance gets complicated
           - legal terms, specific accounting jargon, etc.
           - I won't venture into this thicket here. It's a specialty
              unto itself, with several dozen major types of instruments
              and derivatives. And of course with big doses of the law.
 
 12.4. Smart Cards
   12.4.1. "What are smart cards and how are they used?"
           + Most smart cards as they now exist are very far from being
              the anonymous digital cash of primary interest to us. In
              fact, most of them are just glorified credit cards.
             - with no gain to consumers, since consumes typically don't
                pay for losses by fraud
             - (so to entice consumes, will they offer inducements?)
           - Can be either small computers, typically credit-card-sized,
              or  just cards that control access via local computers.
           + Tamper-resistant modules, e.g., if tampered with, they
              destroy the important data or at the least give evidence of
              having been tampered with.
             + Security of manufacturing
               - some variant of  "cut-and-choose" inspection of
                  premises
           + Uses of smart cards
             - conventional credit card uses
             - bill payment
             - postage
             - bridge and road tolls
             - payments for items received electronically (not
                necessarily anonymously)
   12.4.2. Visa Electronic Purse
   12.4.3. Mondex
 
 12.5. David Chaum's "DigiCash"
   12.5.1. "Why is Chaum so important to digital cash?"
           - Chaum's name appears frequently in this document, and in
              other Cypherpunk writings. He is without a doubt the
              seminal thinker in this area, having been very nearly the
              first to write about several areas: untraceable e-mail,
              digital cash, blinding, unlinkable credentials, DC-nets,
              etc.
           - I spoke to him at the 1988 "Crypto" conference, telling him
              about my interests, my 'labyrinth' idea for mail-forwarding
              (which he had anticipated in 1981, unbeknownst to me at the
              time), and a few hints about "crypto anarchy." It was clear
              to me that Chaum had thought long and deeply about these
              issues.
           - Chaum's articles should be read by all interested in this
              area. (No, his papers are _not_ "on-line." Please see the
              "Crypto" Proceedings and related materials.)
           - [DIGICASH PRESS RELEASE, "World's first electronic cash
              payment over computer networks," 1994-05-27]
   12.5.2. "What's his motivation?"
           - Chaum appears to be a libertarian, at least on social
              issues, and is very worried about "Big Brother" sorts of
              concerns (recall the title of his 1985 CACM article).
           - His work in Europe has mostly concentrated on unlinkable
              credentials for toll road payments, electronic voting, etc.
              His company, DigiCash, is working on various aspects of
              digital cash.
   12.5.3. "How does his system work?"
           - There have been many summaries on the Cypherpunks list. Hal
              Finney has written at least half a dozen, and others have
              been contributed by Eric Hughes, Karl Barrus, etc. I won't
              be including any of them here....it just takes too many
              pages to explain how digital cash works in detail.
           - (The biggest problem people have with digital cash is in
              not taking the time to understand the basics of the math,
              of blinding, etc. They wrongly assume that "digital cash"
              can be understood by common-sense reasoning about existing
              cash, etc. This mistake has been repeated in several of the
              half-assed proposals for "net cash" and "digi dollars.")
           + Here's the opening few paragraphs from one of Hal's
              explanations, to provide a glimpse:
             - "Mike Ingle asks about digicash.  The simplest system I
                know of that is anonymous is the one by Chaum, Fiat, and
                Naor, which we have discussed here a few times.  The idea
                is that the bank chooses an RSA modulus, and a set of
                exponents e1, e2, e3, ..., where each exponent ei
                represents
                a denomination and possibly a date.  The exponents must
                be relatively prime to (p-1)(q-1).  PGP has a GCD routine
                which can be used to check for valid exponents..
                
                "As with RSA, to each public exponent ei corresponds a
                secret exponent di, calculated as the multiplicative
                inverse of ei mod (p-1)(q-1).  Again, PGP has a routine
                to calculate multiplicative inverses.
                
                "In this system, a piece of cash is a pair (x, f(x)^di),
                where f() is a one-way function.  MD5 would be a
                reasonable choice for f(), but notice that it produces a
                128-bit result.  f() should take this 128-bit output of
                MD5 and "reblock" it to be an multi-precision number by
                padding it; PGP has a "preblock" routine which does this,
                following the PKCS standard.
                
                "The way the process works, with the blinding, is like
                this.  The user chooses a random x.  This should probably
                be at least 64 or 128 bits, enough to preclude exhaustive
                search.  He calculates f(x), which is what he wants the
                bank to sign by raising to the power di.  But rather than
                sending f(x) to the bank directly, the user first blinds
                it by choosing a random number r, and calculating D=f(x)
                * r^ei.  (I should make it clear that ^ is the power
                operator, not xor.)  D is what he sends to the bank,
                along with some information about what ei is, which tells
                the denomination of the cash, and also information about
                his account number."  [Hal Finney, 1993-12-04]
   12.5.4. "What is happening with DigiCash?"
           - "Payment from any personal computer to any other
              workstation, over email or Internet, has been demonstrated
              for the first time, using electronic cash technology. "You
              can pay for access to a database, buy software or a
              newsletter by email, play a computer game over the net,
              receive $5 owed you by a friend, or just order a pizza. The
              possibilities are truly unlimited" according to David
              Chaum, Managing Director of DigiCash TM, who announced and
              demonstrated the product during his keynote address at the
              first conference on the World Wide Web, in Geneva this
              week." [DIGICASH PRESS RELEASE, "World's first electronic
              cash payment over computer networks," 1994-05-27]
           - DigiCash is David Chaum's company, set up to commercialize
              this work. Located near Amsterdam.
           + Chaum is also centrally invovled in "CAFE," a European
              committee investigating ways to deploy digital cash in
              Europe
             - mostly standards, issues of privacy, etc.
             - toll roads, ferries, parking meters, etc.
           - http://digicash.support.nl/
           - info@digicash.nl
           - People have been reporting that their inquiries are not
              being answered; could be for several reasons.
   12.5.5. The Complexities of Digital Cash
           - There is no doubt as to the complexity: many protocols,
              semantic confusion, many parties, chances for collusion,
              spoofing, repudiation, and the like. And many derivative
              entities: agents, escrow services, banks.
           - There's no substitute for _thinking hard_ about various
              scenarios. Thinking about how to arrange off-line clearing,
              how to handle claims of people who claim their digital
              money was stolen, people who want various special kinds of
              services, such as receipts, and so on. It's an ecology
              here, not just a set of simple equations.
 
 12.6. Online and Offline Clearing, Double Spending
   12.6.1. (this section still under construction)
   12.6.2. This is one of the main points of division between systems.
   12.6.3. Online Clearing
           - (insert explanation)
   12.6.4. Offline Clearing
           - (insert explanation)
   12.6.5. Double spending
           - Some approaches involve constantly-growing-in-size coins at
              each transfer, so who spent the money first can be deduced
              (or variants of this). And N. Ferguson developed a system
              allowing up to N expenditures of the same coin, where N is
              a parameter. [Howard Gayle reminded me of this, 1994-08-29]
           - "Why does everyone think that the law must immediately be
              invoked when double spending is detected?....Double
              spending is an informational property of digital cash
              systems. Need we find malicious intent in a formal
              property?  The obvious moralism about the law and double
              spenders is inappropriate.  It evokes images of revenge and
              retribution, which are stupid, not to mention of negative
              economic value." [Eric Hughes, 1994-08-27]  (This also
              relates to Eric's good point that we too often frame crypto
              issue in terms of loaded terms like "cheating," "spoofing,"
              and "enemies," when more neutral terms would carry less
              meaning-obscuring baggage and would not give our "enemies"
              (:-}) the ammunition to pass laws based on such terms.)
   12.6.6. Issues
           + Chaum's double-spending detection systems
             - Chaum went to great lengths to develop system which
                preserve anonymity for single-spending instances, but
                which break anonymity and thus reveal identity for double-
                spending instances. I'm not sure what market forces
                caused him to think about this as being so important, but
                it creates many headaches. Besides being clumsy, it
                require physical ID, it invokes a legal system to try to
                collect from "double spenders," and it admits the
                extremely serious breach of privacy by enabling stings.
                For example, Alice pays Bob a unit of money, then quickly
                Alice spends that money before Bob can...Bob is then
                revealed as a "double spender," and his identity revealed
                to whomver wanted it...Alice, IRS, Gestapo, etc. A very
                broken idea. Acceptable mainly for small transactions.
           +  Multi-spending vs. on-line clearing
             - I favor on-line clearing. Simply put: the first spending
                is the only spending. The guy who gets to the train
                locker where the cash is stored is the guy who gets it.
                This ensure that the burden of maintaining the secret is
                on the secret holder.
             - When Alice and Bob transfer money, Alice makes the
                transfer, Bob confirms it as valid (or verifies that his
                bank has received the deposit), and the transaction is
                complete.
             - With network speeds increasing dramatically, on-line
                clearing should be feasible for most transactions. Off-
                line systems may of course be useful, especially for
                small transactions, the ones now handled with coins and
                small bills.
           -
   12.6.7. "How does on-line clearing of anonymous digital cash work?"
           - There's a lot of math connected with blinding,
              exponentions, etc. See Schneier's book for an introduction,
              or the various papers of Chaum, Brands, Bos, etc.
           - On-line clearing is similar to two parties in a transaction
              exchanging goods and money. The transaction is clearled
              locally, and immediately. Or they could arrange transfer of
              funds at a bank, and the banker could tell them over the
              phone that the transaction has cleared--true "on-line
              clearing." Debit cards work this way, with money
              transferred effectively immediately out of one account and
              into another. Credit cards have some additional wrinkles,
              such as the credit aspect, but are basically still on-line
              clearing.
           - Conceptually, the guiding principle idea is simple: he who
              gets to the train locker where the cash is stored *first*
              gets the cash. There can never be "double spending," only
              people who get to the locker and find no cash inside.
              Chaumian blinding allows the "train locker" (e.g., Credit
              Suisse) to give the money to the entity making the claim
              without knowing how the number correlates to previous
              numbers they "sold" to other entities. Anonymity is
              preserved, absolutely. (Ignoring for this discussion issues
              of cameras watching the cash pickup, if it ever actually
              gets picked up.)
           - Once the "handshaking" of on-line clearing is accepted,
              based on the "first to the money gets it" principle, then
              networks of such clearinghouses can thrive, as each is
              confident about clearing. (There are some important things
              needed to provide what I'll dub "closure" to the circuit.
              People need to ping the system, depositing and withdrawing,
              to establish both confidence and cover. A lot like remailer
              networks. In fact, very much like them.)
           - In on-line clearing, only a number is needed to make a
              transfer. Conceptually, that is. Just a number. It is up to
              the holder of the number to protect it carefully, which is
              as it should be (for reasons of locality, or self-
              responsibility, and because any other option introduces
              repudiation, disavowal, and the "Twinkies made me do it"
              sorts of nonsense). Once the number is transferred and
              reblinded, the old number no longer has a claim on the
              money stored at Credit Suisse, for example. That money is
              now out of the train locker and into a new one. (People
              always ask, "But where is the money, really?" I see digital
              cash as *claims* on accounts in existing money-holding
              places, typically banks. There are all kinds of "claims"--
              Eric Hughes has regaled us with tales of his explorations
              of the world of commericial paper. My use of the term
              "claim" here is of the "You present the right number, you
              get access" kind. Like the combination to a safe. The train
              locker idea makes this clearer, and gets around the
              confusion about "digimarks" of "e$" actually _being_ any
              kind of money it and of itself.)
 
 12.7. Uses for Digital Cash
   12.7.1. Uses for digital cash?
           - Privacy protection
           - Preventing tracking of movements, contacts, preferences
           + Illegal markets
             - gambling
             - bribes, payoffs
             - assassinations and other contract crimes
             - fencing, purchases of goods
           + Tax avoidance
             - income hiding
             - offshore funds transfers
             - illegal markets
           - Online services, games, etc.
           + Agoric markets, such as for allocation of computer
              resources
             - where programs, agents "pay" for services used, make
                "bids" for future services, collect "rent," etc.
           + Road tolls, parking fees, where unlinkablity is desired.
              This press release excerpt should give the flavor of
              intended uses for road tolls:
             - "The product was developed by DigiCash TM Corporation's
                wholly owned Dutch subsidiary, DigiCash TM BV. It is
                related to the firm's earlier released product for road
                pricing, which has been licensed to Amtech TM
                Corporation, of Dallas, Texas, worldwide leader in
                automatic road toll collection. This system allows
                privacy protected payments for road use at full highway
                speed from a smart card reader affixed to the inside of a
                vehicle. Also related is the approach of the EU supported
                CAFE project, of which Dr. Chaum is Chairman, which uses
                tamper-resistant chips inserted into electronic wallets."
                [DIGICASH PRESS RELEASE, "World's first electronic cash
                payment over computer networks," 1994-05-27]
   12.7.2. "What are some motivations for anonymous digital cash?"
           + Payments that are unlinkable to identity, especially for
              things like highway tolls, bridge tolls, etc.
             - where linkablity would imply position tracking
             - (Why not use coins? This idea is for "smart card"-type
                payment systems, involving wireless communication.
                Singapore planned (and perhaps has implemented) such a
                system, except there were no privacy considerations.)
           + Pay for things while using pseudonyms
             - no point in having a pseudonym if the payment system
                reveals one's identity
           + Tax avoidance
             - this is the one the digicash proponents don't like to
                talk about too loudly, but it's obviously a time-honored
                concern of all taxpayers
           + Because there is no compelling reason why money should be
              linked to personal identity
             - a general point, subsuming others
 
 12.8. Other Digital Money Systems
   12.8.1. "There seem to be many variants....what's the story?"
           - Lots of confusion. Lots of systems that are not at all
              anonymous, that are just extensions of existing systems.
              The cachet of digital cash is such that many people are
              claiming their systems are "digital cash," when of course
              they are not (at least not in the Chaum/Cypherpunk sense).
           - So, be careful. Caveat emptor.
   12.8.2. Crypto and Credit Cards (and on-line clearing)
           + Cryptographically secure digital cash may find a major use
              in effectively extending the modality of credit cards to
              low-level, person-to-person transactions.
             - That is, the convenience of credit cards is one of their
                main uses (others being the advancing of actual credit,
                ignored here). In fact, secured credit cards and debit
                cards don't offer this advancement of credit, but are
                mainly used to accrue the "order by phone" and "avoid
                carrying cash" advantages.
             - Checks offer the "don't carry cash" advantage, but take
                time to clear. Traveller's checks are a more pure form of
                this.
             - But individuals (like Alice and Bob) cannot presently use
                the credit card system for mutual transactions. I'm not
                sure of all the reasons. How might this change?
             - Crypto can allow unforgeable systems, via some variant of
                digital signatures. That is, Alice can accept a phoned
                payment from Bob without ever being able to sign Bob's
                electronic signature herself.
           - "Crypto Credit Cards" could allow end users (customers, in
              today's system) to handle transactions like this, without
              having merchants as intermediaries.
           - I'm sure the existing credit card outfits would have
              something to say about this, and there may be various
              roadblocks in the way. It might be best to buy off the VISA
              and MasterCard folks by working through them. (And they
              probably have studied this issue; what may change their
              positions is strong crypto, locally available to users.)
           - (On-line clearing--to prevent double-spending and copying
              of cash--is an important aspect of many digital cash
              protocols, and of VISA-type protocols. Fortunately,
              networks are becoming ubiquitous and fast. Home use is
              still a can of worms, though, with competing standards
              based on video cable, fiber optics, ISDN, ATM, etc.)
   12.8.3. Many systems being floated. Here's a sampling:
           + Mondex
             - "Unlike most other electronic purse systems, Mondex, like
                cash, is anonymous.  The banks that issue Mondex cards
                will not be able to keep track of who gets the payments.
                Indeed, it is the only system in which two card holders
                can transfer money to each other.
                
                ""If you want to have a product that replaces cash, you
                have to do everything that cash does, only better,"
                Mondex's senior executive, Michael Keegan said.  "You can
                give money to your brother who gives it to the chap that
                sells newspapers, who gives it to charity, who puts it in
                the bank, which has no idea where it's been.  That's what
                money is."" [New York Times, 1994-09-06, provided by John
                Young]
           + CommerceNet
             - allows Internet users to buy and sell goods.
             - "I read in yesterday's L.A. Times about something called
                CommerceNet, where sellers and buyers of workstation
                level equipment can meet and conduct busniess....Near the
                end of the article, they talked about a proposed method
                for  exchanging "digital signatures" via Moasic (so that
                buyers and sellers could _know_ that they were who they
                said they were) and that they were going to "submit it to
                the Internet Standards body"" [Cypher1@aol.com, 1994-06-
                23]
           + NetCash
             - paper published at 1st ACM Conference on Computer and
                Communications Security, Nov. 93, available via anonymous
                ftp from PROSPERO.ISI.EDU as /pub/papers/security/netcash-
                cccs93.ps.Z
             - "NetCash: A design for practical electronic currency on
                the Internet  ... Gennady Medvinsky and Clifford Neuman
                
                "NetCash is a framework that supports realtime electronic
                payments with provision of anonymity over an unsecure
                network.  It is designed to enable new types of services
                on the Internet which have not been practical to date
                because of the absence of a secure, scalable, potentially
                anonymous payment method.
                
                "NetCash strikes a balance between unconditionally
                anonymous electronic currency, and signed instruments
                analogous to checks that are more scalable but identify
                the principals in a transaction.  It does this by
                providing the framework within which proposed electronic
                currency protocols can be integrated with the scalable,
                but non-anonymous, electronic banking infrastructure that
                has been proposed for routine transactions."
             + Hal Finney had a negative reaction to their system:
               - "I didn't think it was any good.  They have an
                  incredibly simplistic model, and their "protocols" are
                  of the order, A sends the bank some paper money, and B
                  sends A some electronic cash in return.....They don't
                  even do blinding of the cash.  Each piece of cash has a
                  unique serial number which is known to the currency
                  provider.  This would of course allow matching of
                  withdrawn and deposited coins....These guys seem to
                  have read the work in the field (they reference it) but
                  they don't appear to have understood it." [Hal Finney,
                  1993-08-17]
           + VISA Electronic Purse
             - (A lot of stuff appeared on this, including listings of
                the alliance partners (like Verifone), the technology,
                the plans for deployment, etc. I regret that I can't
                include more here. Maybe when this FAQ is a Web doc, more
                can be included.)
             - "PERSONAL FINANCE - Seeking the Card That Would Create A
                Cashless World. The Washington Post, April 03, 1994,
                FINAL Edition By: Albert B. Crenshaw, Washington Post ...
                
                "Now that credit cards are in the hands of virtually
                every living, breathing adult  in  the  country-not to
                mention a lot of children and the occasional family  pet-
                and  now  that  almost  as  many people  have  ATM cards,
                card companies are wondering where future growth will
                come from.
                
                "At *Visa* International, the answer is: Replace cash
                with plastic.
                
                "Last month,  the  giant  association  of  card issuers
                announced it had formed a coalition of banking and
                technology companies to develop technical standards  for
                a  product it dubbed the "Electronic Purse," a plastic
                card meant to replace coins and bills in small
                transactions."  [provided by Duncan Frissell, 1994-04-05]
             - The talk of "clearinghouses" and the involvement of VISA
                International and the Usual Suspects suggest
                identity-blinding protocols are not in use. I also see no
                mention of DigiCash, or even RSA (but maybe I missed that-
                -and the presence of RSA would not necessairly mean
                identity-blinding protocols were being planned).
                
                Likely Scenario: This is *not* digital cash as we think
                of it. Rather, this is a future evolution of the cash ATM
                card and credit card, optimized for faster and cheaper
                clearing.
                
                Scary Scenario: This could be the vehicle for the long-
                rumored "banning of cash." (Just because conspiracy
                theorists and Number of the Beast Xtian fundamentalists
                belive it doesn't render it implausible.)
             - Almost nothing of interest for us. No methods for
                anonymity. Make no mistake, this is not the digital cash
                that Cypherpunks espouse. This gives the credit agencies
                and the government (the two work hand in hand) complete
                traceability of all purchases, automatic reporting of
                spending patterns, target lists for those who frequent
                about-to-be-outlawed businesses, and invasive
                surveillance of all inter-personal economic transactions.
                This is the AntiCash. Beware the Number of the AntiCash.
   12.8.4. Nick Szabo:
           - "Internet commercialization in itself is a _huge_ issue
              full of pitfall and  opportunity: Mom & Pop BBS's,
              commercial MUDs, data banks, for-profit pirate and porn
              boards, etc. are springing  up everywhere like weeds,
              opening a vast array of both needs of privacy and ways to
              abuse privacy.  Remailers, digital cash, etc. won't become
              part of this Internet commerce way of life unless they are
              deployed soon, theoretical flaws and all, instead of
              waiting until The Perfect System comes along.  Crypto-
              anarchy in the real world will be messy, "nature red in
              tooth and claw", not all nice and clean like it says in the
              math books.  Most of thedebugging will be done not in any
              ivory tower, but by the bankruptcy of businesses who
              violate their customer's privacy, the confiscation of BBS
              operators who stray outside the laws of some jurisdication
              and screw up their privacy arrangements, etc. Anybody who
              thinks they can flesh out a protocol in secret and then
              deploy it, full-blown and working, is in for a world of
              hurt.  For those who get their Pretty Good systems out
              there and used, there is vast potential for business growth
              -- think of the $trillions confiscated every year by
              governments around the world, for example." [Nick Szabo,
              1993-8-23]
   12.8.5. "What about _non-anonymous_ digital cash?"
           - a la the various extensions of existing credit and debit
              cards, traveller's checks, etc.
           + There's still a use for this, with several motivations"
             * for users, it may be _cheaper_ (lower transaction costs)
                than fully anonymous digital cash
             * for banks, it may also be cheaper
             * users may wish audit trails, proof, etc.
             * and of course governments have various reasons for
                wanting traceable cash systems
               - law enforcement
               - taxes, surfacing the underground economy
   12.8.6. Microsoft plans to enter the home banking business
           - "PORTLAND, Ore. (AP) -- Microsoft Corp. wants to replace
              your checkbook with a home computer that lets the bank do
              all the work of recording checks, tallying up credit card
              charges and paying bills.... The service also tracks credit
              card accounts, withdrawals from automated teller machines,
              transfers from savings or other accounts, credit lines,
              debit cards, stocks and other investments, and bill
              payments." [Associated Press, 1994-07-04]
           - Planned links with a consortium of banks, led by U.S.
              Bancorp, using its "Money" software package.
           - Comment: Such moves as this--and don't forget the cable
              companies--could result in a rapid transition to a form of
              home banking and "digital money." Obviously this kind of
              digital money, as it is being planned today, is very from
              the kind of digital cash that interests us. In fact, it is
              the polar opposite of what we want.
   12.8.7. Credit card clearing...individuals can't use the system
           - if something nonanonymous like credit cards cannot be used
              by end users (Alice and Bob), why would we expect an
              anonymous version of this would be either easier to use or
              more possible?
           - (And giving users encrypted links to credit agencies would
              at least stop the security problems with giving credit card
              numbers out over links that can be observed.)
           - Mondex claims their system will allow this kind of person-
              to-person transfer of anonymous digital cash (I'll believe
              it when I see it).
 
 12.9. Legal Issues with Digital Cash
   10.8.1. "What's the legal status of digital cash?"
           - It hasn't been tested, like a lot of crypto protocols. It
              may be many years before these systems are tested.
   10.8.2. "Is there a tie between digital cash and money laundering?"
           - There doesn't have to be, but many of us believe the
              widespread deployment of digital, untraceable cash will
              make possible new approaches
           - Hence the importance of digital cash for crypto anarchy and
              related ideas.
           - (In case it isn't obvious, I consider money-laundering a
              non-crime.)
   10.8.3. "Is it true the government of the U.S. can limit funds
            transfers outside the U.S.?"
           - Many issues here. Certainly some laws exist. Certainly
              people are prosecuted every day for violating currency
              export laws. Many avenues exist.
           - "LEGALITY - There isn't and will never be a law restricting
              the sending of funds outside the United States.  How do I
              know?  Simple.  As a country dependant on international
              trade (billions of dollars a year and counting), the
              American economy would be destroyed." [David Johnson,
              privacy@well.sf.ca.us, "Offshore Banking & Privacy,"
              alt.privacy, 1994-07-05]
   10.8.4. "Are "alternative currencies" allowed in the U.S.? And what's
            the implication for digital cash of various forms?
           - Tokens, coupons, gift certificates are allowed, but face
              various regulations. Casino chips were once treated as
              cash, but are now more regulated (inter-casino conversion
              is no longer allowed).
           - Any attempt to use such coupons as an alternative currency
              face obstacles.  The coupons may be allowed, but heavily
              regulated (reporting requirements, etc.).
           - Perry Metzger notes, bearer bonds are now illegal in the
              U.S. (a bearer bond represented cash, in that no name was
              attached to the bond--the "bearer" could sell it for cash
              or redeem it...worked great for transporting large amounts
              of cash in compact form).
           + Note: Duncan Frissell claims that bearer bonds are _not_
              illegal.
             - "Under the Tax Equity and Fiscal Responsibility Act of
                1982 (TEFRA), any interest payments made on *new* issues
                of domestic bearer bonds are not deductible as an
                ordinary and necessary business expense so none have been
                issued since then.  At the same time, the Feds
                administratively stopped issuing treasury securities in
                bearer form.  Old issues of government and corporate debt
                in bearer form still exist and will exist and trade for
                30 or more years after 1982.  Additionally, US residents
                can legally buy foreign bearer securities." [Duncan
                Frissell, 1994-08-10]
             - Someone else has a slightly different view: "The last US
                Bearer Bond issues mature in 1997. I also believe that to
                collect interest, and to redeem the bond at maturity, you
                must give your name and tax-id number to the paying
                agent. (I can check with the department here that handles
                it if anyone is interested in the pertinent OCC regs that
                apply)"  [prig0011@gold.tc.umn.edu, 1994-08-10]
             - I cite this gory detail to give readers some idea about
                how much confusion there is about these subjects. The
                usual advice is to "seek competent counsel," but in fact
                most lawyers have no clear ideas about the optimum
                strategies, and the run-of-the-mill advisor may mislead
                one dangerously. Tread carefully.
           - This has implications for digital cash, of course.
   10.8.5. "Why might digital cash and related techologies take hold
            early in illegal markets? That is, will the Mob be an early
            adopter?"
           - untraceability needed
           - and reputations matter to them
           - they've shown in the past that they will try new
              approaches, a la the money movements of the drug cartels,
              novel methods for security, etc.
   10.8.6. "Electronic cash...will it have to comply with laws, and
            how?"
           - Concerns will be raised about the anonymity aspects, the
              usefulness for evading taxes and reporting requirements,
              etc.
           - a messy issue, sure to be debated and legislated about for
              many years
           + split the cash into many pieces...is this "structuring"? is
              it legal?
             - some rules indicate the structuring per se is not
                illegal, only tax evasion or currency control evasion
             - what then of systems which _automatically_, as a basic
                feature, split the cash up into multiple pieces and move
                them?
   10.8.7. Currency controls, flight capital regulations, boycotts,
            asset seizures, etc.
           - all are pressures to find alternate ways for capital to
              flow
           - all add to the lack of confidence, which, paradoxically to
              lawmakers, makes capital flight all the more likely
   10.8.8. "Will banking regulators allow digital cash?"
           - Not easily, that's for sure. The maze of regulations,
              restrictions, tax laws, and legal rulings is daunting. Eric
              Hughes spent a lot of time reading up on the laws regarding
              banks, commercial paper, taxes, etc., and concluded much
              the same. I'm not saying it's impossible--indeed, I believe
              it will someday happen, in some form--but the obstacles are
              formidable.
           + Some issues:
             + Will such an operation be allowed to be centered or based
                in the U.S.?
               - What states? What laws? Bank vs. Savings and Loan vs.
                  Credit Union vs. Securities Broker vs. something else?
             + Will customers be able to access such entities offshore,
                outside the U.S.?
               - strong crypto makes communication possible, but it may
                  be difficult, not part of the business fabric, etc.
                  (and hence not so useful--if one has to send PGP-
                  encrypted instructions to one's banker, and can't use
                  the clearing infrastructure....)
             + Tax collection, money-laundering laws, disclosure laws,
                "know your customer" laws....all are areas where a
                "digital bank" could be shut down forthwith. Any bank not
                filling out the proper forms (including mandatory
                reporting of transactions of certain amounts and types,
                and the Social Security/Taxpayer Number of customers)
                faces huge fines, penalties, and regulatory sanctions.
               - and the existing players in the banking and securities
                  business will not sit idly by while newcomers enter
                  their market; they will seek to force newcomers to jump
                  through the same hoops they had to (studies indicate
                  large corporations actually _like_ red tape, as it
                  helps them relative to smaller companies)
           - Concluson: Digital banks will not be "launched" without a
              *lot* of work by lawyers, accountants, tax experts,
              lobbyists, etc. "Lemonade stand digital banks" (TM) will
              not survive for long. Kids, don't try this at home!
           - (Many new industries we are familiar with--software,
              microcomputers--had very little regulation, rightly so. But
              the effect is that many of us are unprepared to understand
              the massive amount of red tape which businesses in other
              areas, notably banking, face.)
   10.8.9. Legal obstacles to digital money. If governments don't want
            anonymous cash, they can make things tough.
           + As both Perry Metzger and Eric Hughes have said many times,
              regulations can make life very difficult. Compliance with
              laws is a major cost of doing business.
             - ~"The cost of compliance in a typical USA bank is 14% of
                operating costs."~ [Eric Hughes, citing an "American
                Banker" article, 1994-08-30]
           + The maze of regulations is navigable by larger
              institutions, with staffs of lawyers, accountants, tax
              specialists, etc., but is essentially beyond the
              capabilities of very small institutions, at least in the
              U.S.
             - this may or may not remain the case, as computers
                proliferate. A "bank-in-a-box" program might help. My
                suspicion is that a certain size of staff is needed just
                to handle the face-to-face meetings and hoop-jumping.
           + "New World Order"
             - U.S. urging other countries to "play ball" on banking
                secrecy, on tax evasion extradition, on immigration, etc.
             - this is closing off the former loopholes and escape
                hatches that allowed people to escape repressive
                taxation...the implications for digital money banks are
                unclear, but worrisome.

12.10. Prospects for Digital Cash Use
  12.10.1. "If digital money is so great, why isn't it being used?"
           - Hasn't been finished. Protocols are still being researched,
              papers are still being published. In any single area, such
              as toll road payments, it may  be possible to deploy an
              application-specific system, but there is no "general"
              solution (yet). There is no "digital coin" or unforgeable
              object representing value, so the digital money area is
              more similar to the similarly nonsimple markets in
              financial instruments, commercial papers, bonds, warrants,
              checks, etc. (Areas that are not inherently simple and that
              have required lots of computerization and communications to
              make manageable.)
           - Flakiness of Nets. Systems crash, mail gets delayed
              inexplicably, subscriptions to lists get lunched, and all
              sorts of other breakages occur. Most interaction on the
              Nets involves a fair amount of human adaptation to changing
              conditions, screwups, workarounds, etc. These are not
              conditions that inspire confidence in automated money
              systems!
           - Hard to Use. Few people will use systems that require
              generating code, clients, etc. Semantic gap (generating
              stuff on a Unix workstation is not at all like taking one's
              checkbook out). Protocols in crypto are generally hard to
              use and confusing.
           - Lack of compelling need. Although people have tried various
              experiments with digital money tokens or coupons (Magic
              Money/Tacky Tokens, the HeX market, etc.), there is little
              real world incentive to experiment with them. And most of
              the denominated tokens are for truly trivial amounts of
              money, not for anything worth spending time learning. No
              marketplace for buyers to "wander around in." (You don't
              buy what you don't see.)
           - Legal issues. The IRS does not look favorably on
              alternative currencies, especially if used in attempts to
              bypass ordinary tax collection schemes. This and related
              legal issues (redemptions into dollars) put a roadblock in
              front of serious plans to use digital money.
           - Research Issues. Not all problems resolved. Still being
              developed, papers being published. Chaum's system does not
              seem to be fully ready for deployment, certainly not
              outside of well-defined vertical markets.
  12.10.2. "Why isn't digital money in use?"
           - The Meta Issue: *what* digital money? Various attempts at
              digital cash or digital money exist, but most are flawed,
              experimental, crufty, etc. Chaum's DigiCash was announced
              (Web page, etc.), but is apparently not even remotely
              usable.
           + Practical Reasons:
             - nothing to buy
             - no standard systems that are straightforward to use
             - advantages of anonymity and untraceability are seldom
                exploited
           - The Magic Money/Tacky Tokens experiment on the Cypherpunks
              list is instrucive. Lots of detailed work, lots of posts--
              and yet not used for anything (granted, there's not much
              being bought and sold on the List, so...).
           - Scenario for Use in the Near Future: A vertical
              application, such as a bridge toll system that offers
              anonymity. In a vertical app, the issues of compatibility,
              interfaces, and training can be managed.
  12.10.3. "why isn't digital cash being used?"
           + many reasons, too many reasons!
             + hard issues, murky issues
               - technical developments not final, Chaum, Brands, etc.
             + selling the users
               - who don't have computers, PDAs, the means to do the
                  local computations
               - who want portable versions of the same
             + The infrastructure for digital money (Chaum anonymous-
                style, and variants, such as Brands) does not now exist,
                and may not exist for several more years. (Of course, I
                thought it would take "several more years" back in 1988,
                so what do I know?)
               - The issues are familiar: lack of standards, lack of
                  protocols, lack of customer experience, and likely
                  regulatory hurdles. A daunting prospect.
               - Any "launches" will either have to be well-funded, well-
                  planned, or done sub rosa, in some quasi-legal or even
                  illegal market (such as gambling).
           - "The american people keep claiming in polls that they want
              better privacy protection, but the fact is that most aren't
              willing to do anything about it: it's just a preference,
              not a solid imperative.  Until something Really Bad happens
              to many people as a result of privacy loss, I really don't
              think much will be done that requires real work and
              inconvenience from people, like moving to something other
              than credit cards for long-distance transactions... and
              that's a tragedy."[L. Todd Masco , 1994-08-20]
  12.10.4. "Is strong crypto needed for digital cash?"
           - Yes, for the most bulletproof form, the form of greatest
              interest to us and especially for agents, autonomous
              systems
           + No, for certain weak versions (non-cryptographic methods of
              security, access control, biometric security, etc. methods)
             - for example, Internet billing is not usually done with
                crypto
             - and numbered Swiss accounts can be seen as a weak form of
                digital cash (with some missing features)
             - "warehouse receipts," as in gold or currency shipments
  12.10.5. on why we may not have it for a while, from a non-Cypherpunk
            commenter:
           - "Government requires information on money flows, taxable
              items, and large financial transactions.....As a result, it
              would be nearly impossible to set up a modern anonymous
              digital cash system, despite the fact that we have the
              technology.....I think we have more of a right to privacy
              with digicash transactions, and I also think there is a
              market for anonymous digicash systems. " [Thomas Grant
              Edwards. talk.politics.crypto, 1994-09-06]
  12.10.6. "Why do a lot of schemes for things like digital money have
            problems on the Net?
           + Many reasons
             - lack of commercial infrastructure in general on the
                Net...people are not used to buying things, advertising
                is discouraged (or worse), and almost everything is
                "free."
             - lack of robustness and completeness in the various
                protocols: they are "not ready for prime time" in most
                cases (PGP is solid, and some good shells exist for PGP,
                but the many other crypto protocols are mostly not
                implemented at all, at least not widely).
             + The Net runs "open-loop," as a store-and-forward delivery
                system
               - The Net is mostly a store-and-forward netword, at least
                  at the granularity seen by the user in sending
                  messages, and hence is "open loop." Messages may or may
                  not be received in a timely way, and there is little
                  opportunity for negotiaton on a real-time basis.
               - This open-loop nature usually works...messages get
                  through most of the time. And the "message in a bottle"
                  nature fits in with anonymous remailers (with
                  latency/delay), with message pools, and with other
                  schemes to make traffic analysis harder. A "closed-
                  loop," responsive system is likelier to be traffic-
                  analyzed by correlation of packets, etc.
               - but the sender does not know if it gets through (return
                  receipts not commonly implemented...might be a nice
                  feature to incorporate; agent-based systems
                  (Telescript?) will certainly do this)
               - this open-loop nature makes protocols, negotiation,
                  digital cash very tough to use--too much human
                  intervention needed
               - Note: These comments apply mainly to _mail_ systems,
                  which is where most of us have experimented with these
                  ideas. Non-mail systems, such as Mosaic or telnet or
                  the like, have better or faster feedback mechanisms and
                  may be preferable for implementation of Cypherpunks
                  goals. It may be that the natural focus on mailing
                  lists, e-mail, etc., has distracted us. Perhaps a focus
                  on MUDs, or even on ftp, would have been more
                  fruitful...but we're a mailing list, and most people
                  are much more familiar with e-mail than with archie or
                  gopher or WAIS, etc.
             - The legal and regulatory obstacles to a real system, used
                for real transactions, are formidable. (The obstacles to
                a "play" system are not so severe, but then play systems
                tend not to get much developer attention.)
  12.10.7. Scenario for deployment of digital cash
           - Eric Hughes has spent time looking into this. Too many
              issues to go into here, but he had this interesting
              scenario, repeated almost in toto here:
           - "It's very unlikely that a USA bank will be the one to
              deploy anonymous digital dollars first.  It's much more
              likely that the first dollar digital cash will be issued
              overseas, possibly London.  By the same token, the non-
              dollar regulation on banks in this country is not the same
              as the dollar regulation, so it's quite possible that the
              New York banks may be the first issuers of digital cash, in
              pounds sterling, say.
              
              "There will be two stages in actually deploying digital
              cash.  By digital cash, here, I mean a retail phenomenon,
              available anybody. The first will be to digitize money, and
              the second will be to anonymize it.  Efforts are already
              well underway to make more-or-less secure digital funds
              transfers with reasonably low transaction fees (not
              transaction costs, which are much more than just fees).
              These efforts, as long as they retain some traceability,
              will almost certainly succeed first in the marketplace,
              because (and this is vital) the regulatory environment
              against anonymity is not compromised.
              
              "Once, however, money has been digitized, one of the
              services available for purchase can be the anonymous
              transfer of funds.  I expect that the first digitization of
              money won't be fully fungible.  For example, if you allow
              me to take money out of your checking account by automatic
              debit, there is risk that the money won't be there when I
              ask for it.  Therefore that kind of money won't be
              completely fungible, because money authorized from one
              person won't be completely identical with money from
              another.  It may be a risk issue, it may be a timeliness
              issue, it may be a fee issue; I don't know, but it's
              unlikely to be perfect.
              
              "Now, as the characteristic size of a business decreases,
              the relative costs of dealing with whatever imperfection
              there is will be greater. To wit, the small player will
              still have some problem getting paid, although certainly
              less than now.  Digital cash solves many of these problems.
              The clearing is immediate and final (no transaction
              reversals).  The number of entities to deal with is greatly
              reduced, hopefully to one.  The need and risk and cost of
              accounts receivables is eliminated.  It's anonymous.  There
              will be services which will desire these advantages, enough
              to support a digital cash infrastructure. [Eric Hughes,
              Cypherpunks list, 1994-08-03]

12.11. Commerce on the Internet
  12.11.1. This has been a brewing topic for the past couple of years.
            In 1994 thing heated up on several fronts:
           - DigiCash announcement
           - NetMarket announcement
           - various other systems, including Visa Electronic Purse
  12.11.2. I have no idea which ones will succeed...
  12.11.3. NetMarket
           - Mosaic connections, using PGP
           + "The NetMarket Company is now offering PGP-encrypted Mosaic
              sessions for securely transmitting credit card information
              over the Internet.  Peter Lewis wrote an article on
              NetMarket on page D1 of today's New York Times (8/12/94).
              For more information on NetMarket, connect to
              http://www.netmarket.com/  or,  telnet netmarket.com." [
              Guy H. T. Haskin <guy@netmarket.com>, 1994-08-12]
             - Uses PGP. Hailed by the NYT as the first major use of
                crypto for some form of digital money, but this is not
                correct.
  12.11.4. CommerceNet
           - allows Internet users to buy and sell goods.
           - "I read in yesterday's L.A. Times about something called
              CommerceNet, where sellers and buyers of workstation level
              equipment can meet and conduct busniess....Near the end of
              the article, they talked about a proposed method for
              exchanging "digital signatures" via Moasic (so that buyers
              and sellers could _know_ that they were who they said they
              were) and that they were going to "submit it to the
              Internet Standards body"" [Cypher1@aol.com, 1994-06-23]
  12.11.5. EDI, purchase orders, paperwork reduction, etc.
           - Nick Szabo is a fan of this approach
  12.11.6. approaches
           - send VISA numbers in ordinary mail....obviously insecure
           - send VISA numbers in encrypted mail
           + establish two-way clearing protocols
             - better ensures that recipient will fulfill service...like
                a receipt that customer signs (instead of the "sig taken
                over the phone" approach)
             - various forms of digital money
  12.11.7. lightweight vs. heavyweight processes for Internet commerce
           - Chris Hibbert
           - and the recurring issue of centralized vs. decentralized
              authentication and certification

12.12. Cypherpunks Experiments ("Magic Money")
  12.12.1. What is Magic Money?
           - "Magic Money is a digital cash system designed for use over
              electronic mail. The system is online and untraceable.
              Online means that each transaction involves an exchange
              with a server, to prevent double-spending. Untraceable
              means that it is impossible for anyone to trace
              transactions, or to match a withdrawal with a deposit, or
              to match two coins in any way."
              
              "The system consists of two modules, the server and the
              client. Magic Money uses the PGP ascii-armored message
              format for all communication between the server and client.
              All traffic is encrypted, and messages from the server to
              the client are signed. Untraceability is provided by a
              Chaum-style blind signature. Note that the blind signature
              is patented, as is RSA. Using it for experimental purposes
              only shouldn't get you in trouble.
              
              "Digicash is represented by discrete coins, the
              denominations of which are chosen by the server operator.
              Coins are RSA-signed, with a different e/d pair for each
              denomination. The server does not store any money. All
              coins are stored by the client module. The server accepts
              old coins and blind- signs new coins, and checks off the
              old ones on a spent list."
              [...rest of excellent summary elided...highly recommended
              that you dig it up (archives, Web site?) and read it]
              [Pr0duct Cypher, Magic Money Digicash System, 1992-02-04]
           + Magic Money
             - ftp://csn.org/pub/mpj/crypto_XXXXXX (or something like
                that) <Derek Atkins, 4-7-94>
             - ftp:csn.org//mpj/I_will_not_export/crypto_???????/pgp_too
                ls  <Michael Paul Johnson, 4-7-94>
  12.12.2. Matt Thomlinson experimented with a derivative version called
            "GhostMarks"
  12.12.3. there was also a "Tacky Tokens" derivative
  12.12.4. Typical Problems with Such Experiments
           - Not worth anything...making the money meaningful is an
              obstacle to be overcome
           - If worth anything, not worth the considerable effort to use
              it ("creating Magic Money clients" and other scary Unix
              stuff!)
           - robustness...sites go down, etc.
           - same problems were seen on Extropians list with "HEx"
              exchange and its currency, the "thorne." (I even paid real
              money to Edgar Swank to buy some thorned...alas, the market
              was too thinly traded and the thornes did me no good.)

12.13. Practical Issues and Concerns with Digital Cash
  12.13.1. "Is physical identity proof needed for on-line clearing?"
           - No, not if the cash outlook is taken. Cash is cash. Caveat
              emptor.
           - The "first to the locker" approach causes the bank not to
              particularly care about this, just as a Swiss bank will
              allow access to a numbered account by presentation of the
              number, and perhaps a key. Identity proof *may* be needed,
              depending on the "protocol" they and the customer
              established, but it need not be. And the last thing the
              bank is worried about is being able to "find and prosecute"
              anyone, as there is no way they can be liable for a double
              spending incident. The beauties of local clearing! (Which
              is what gold coins do, and paper money if we really think
              we can pass it on to others.)
  12.13.2. "Is digital cash traceable?"
           - There are several flavors of "digital cash," ranging from
              versions of VISA cards to fully untraceable (Chaumian)
              digital cash.
           - This comes up a lot, with people in Net newsgroups even
              warning others not to use digital cash because of the ease
              of traceability. Not so.
           - "Not the kind proposed by David Chaum and his colleagues in
              the Netherlands. The whole thrust of their research over
              the last decade has been the use of cryptographic
              techniques to make electronic transactions secure from
              fraud while at the same time protecting personal privacy.
              They, and others, have developed a number of schemes for
              UNTRACEABLE digital cash." [Kevin Van Horn,
              talk.politics.crypto, 1994-07-03]
  12.13.3. "Is there a danger that people will lose the numbers that
            they need to redeem money? That someone could steal the
            number and thus steal their money?"
           - Sure. There's the danger that I'll lose my bearer bonds, or
              forget my Swiss bank account number, or lose my treasure
              map to where I buried my money (as Alan Turing supposedly
              did in WW II).
           - People can take steps to limit risk. More secure computers.
              Dongles worn around their necks. Protocols that involve
              biometric authentication to their local computer or key
              storage PDA, etc. Limits on withdrawals per day, etc.
              People can store key numbers with people they trust,
              perhaps encrypted with other keys, can leave them with
              their lawyers, etc. All sorts of arrangements can be made.
              Personal identification is but one of these arrangements.
              Often used, but not essential to the underlyng protocol.
              Again, the Swiss banks (maybe now the Liechtenstein
              anstalts are a better example) don't require physical ID
              for all accounts. (More generally, if Charles wants to
              create a bank in which deposits are made and then given out
              to the first person who sings the right tune, why should we
              care? This extreme example is useful in pointing out that
              _contractual arrangements_ need not involve governmental or
              societal norms about what constitutes proof of identity.)

12.14. Cyberspace and Digital Money
  12.14.1. "You can't eat cyberspace, so what good is digital money?"
           - This comes up a lot. People assume there is no practical
              way to transfer assets, when in fact it is done all the
              time. That is, money flows from the realm of the purely
              "informational" realm to the physcial realm Consultants,
              writers, traders, etc., all use their heads and thereby
              earn real money.
           - Same will apply to cyberspace.
  12.14.2. "How can I remain anonymous when buying physical items using
            anonymous digital cash?'
           - Very difficult. Once you are seen, and your picture can be
              taken( perhaps unknown to you), databases will have you.
              Not much can be done about this.
           - People have proposed schemes for anonymous shipment and
              pickup, but the plain fact is that physical delivery of any
              sort compromises anonymity, just as in the world today.
           - The purpose of anonymous digital cash is partly to at least
              make it more difficult, to not give Big Brother your
              detailed itinerary from toll road movements, movie theater
              payments, etc. To the extent that physical cameras can
              still track cars, people, shipments, etc., anonymous
              digital cash doesn't solve this surveillance problem.

12.15. Outlawing of Cash
  12.15.1. "What are the motivations for outlawing cash?"
           - (Note: This has not happened. Many of us see signs of it
              happening. Others are skeptical.)
           + Reasons for the Elimination of Cash:
             - War on Drugs....need I say more?
             -  surface the underground economy, by withdrawing paper
                currency and forcing all monetary transaction into forms
                that can be easily monitored, regulated, and taxed.
             - tax avoidance, under the table economy (could also be
                motive for tamper-resistant cash registers, with spot
                checks to ensure compliance)
             + welfare, disability, pension, social security auto-
                deposits
               - fraud, double-dipping
               - reduce theft of welfare checks, disability payments,
                  etc....a problem in some locales, and automatic
                  deposit/cash card approaches are being evaluated.
             - general reduction in theft, pickpockets
             - reduction of paperwork: all transfers electronic (could
                be part of a "reinventing government" initiative)
             +  illegal immigrants, welfare cheats, etc. Give everyone a
                National Identity Card (they'll call it something
                different. to make it more palatable, such as "Social
                Services Portable Inventory Unit" or "Health Rights
                Document").
               - (Links to National Health Care Card, to Welfare Card,
                  to other I.D. schemes designed to reduce fraud, track
                  citizen-units, etc.)
             + rationing systems that depend on non-cash transactions
                (as explained elsewhere, market distortions from
                rationing systems generally require identification,
                correlation to person or group, etc.)
               - this rationing can included subsidized prices, denial
                  of access (e.g., certain foods denied to certain
                  people)
  12.15.2. Lest this be considered paranoid ranting, let me point out
            that many actions have already been taken that limit the form
            of money (banking laws, money laundering, currency
            restrictions...even the outlawing of competing currencies
            itself)
  12.15.3. Dangers of outlawing cash
           - Would freeze out all transactions, giving Big Brother
              unprecedented power (unless the non-cash forms were
              anonymous, a la Chaum and the systems we support)
           - Would allow complete traceability....like the cellular
              phones that got Simpson
           - 666, Heinlein, Shockwave Rider, etc.
  12.15.4. Given that there is no requirement for identity to be
            associated with money, we should fight any system which
            proposed to link the two.
  12.15.5. The value of paying cash
           - makes a transaction purely local, resolved on the spot
           - the alternative, a complicated accounting system involving
              other parties, etc., is much less attractive
           - too many transactions these days are no longer handled in
              cash, which increases costs and gets other parties involved
              where they shouldn't be involved.
  12.15.6. "Will people accept the banning of cash?"
           - There was a time when I would've said Americans, at least,
              would've rejected such a thing. Too many memories of
              "Papieren, bitte. Macht schnell!" But I now think most
              Americans (and Europeans) are so used to producing
              documents for every transaction, and so used to using VISA
              cards and ATM cards at gas stations, supermarkets, and even
              at flea markets, that they'll willingly--even eagerly--
              adopt such a system.

12.16. Novel Opportunities
  12.16.1. Encrypted open books, or anonymous auditing
           - Eric Hughes has worked on a scheme using a kind of blinding
              to do "encrypted open books," whereby observers can verify
              that a bank is balancing its books without more detailed
              looks at individual accounts. (I have my doubts about
              spoofs, attacks, etc., but such are always to be considered
              in any new protocol.)
           - "Kent Hastings wondered how an offshore bank could provide
              assurances to depositors.  I wondered the same thing a few
              months ago, and started working on what Perry calls the
              anonymous auditing problem.  I have what I consider to be
              the core of a solution.
              ...The following is long.... [TCM Note: Too long to include
              here. I am including just enough to convince readers that
              some new sorts of banking ideas may come out of
              cryptography.]
              
              "If we use the contents of the encrypted books at the
              organizational boundary points to create suitable legal
              opbligations, we can mostly ignore what goes on inside of
              the mess of random numbers.  That is, even if double books
              were being kept, the legal obligations created should
              suffice to ensure that everything can be unwound if needed.
              This doesn't prevent networks of corrupt businesses from
              going down all at once, but it does allow networks of
              honest businesses to operate with more assurance of
              honesty." [Eric Hughes,  PROTOCOL: Encrypted Open Books,
              1993-08-16]
  12.16.2. "How can software components be sold, and how does crypto
            figure in?"
           + Reusable Software, Brad Cox, Sprague, etc.
             - good article in "Wired" (repeated in "Out of Control")
           - First, certainly software is sold. The issues is why the
              "software components" market has not yet developed, and why
              such specific instances of software as music, art, text,
              etc., have not been sold in smaller chunks.
           + Internet commerce is a huge area of interest, and future
              development.
             - currently developing very slowly
             - lots of conflicting information...several mailing
                lists...lots of hype
           + Digital cash is often cited as a needed enabling tool, but
              I think the answer is more complicated than that.
             - issues of convenience
             - issues of there being no recurring market (as there is
                in, say, the chip business...software doesn't get bought
                over and over again, in increasing unit volumes)

12.17. Loose Ends
  12.17.1. Reasons to have no government involvement in commerce
           - Even a small involvement, through special regulations,
              granted frachises, etc., produces vested interests. For
              example, those in a community who had to wait to get
              building permits want _others_ to wait just as long, or
              longer. Or, businesses that had to meet certain standard,
              even if unreasonable, will demand that new businesses do so
              also. The effect is an ever-widening tar pit of rules,
              restrictions, and delays. Distortions of the market result.
           + Look at how hard it is for the former U.S.S.R. to
              disentangle itself from 75 years of central planning. They
              are now an almost totally Mafia-controlled state (by this I
              mean that "privatization" of formerly non-private
              enterprises benefitted those who had amassed money and
              influence, and that these were mainly the Russian Mafia and
              former or current politicians...the repercussions of this
              "corrupt giveaway" will be felt for decades to come).
             - An encouraging sign: The thriving black market in Russia-
                -which all Cypherpunks of course cheer--will gradually
                displace the old business systems with new ones, as in
                all economies. Eventually the corruptly-bought businesses
                will sink or swim based on merit, and newly-created
                enterprises will compete with them.
  12.17.2. "Purist" Approach to Keys, Cash, Responsibility
           + There are two main approaches to the issue:
             - Key owner is responsible for uses of his key
             - or, Others are responsible
           + There may be mixed situations, such as when a key is
              stolen...but this needs also to be planned-for by the key
              owner, by use of protocols that limit exposure. For
              example, few people will use a single key that accesses
              immediately their net worth...most people will partition
              their holding and their keyed access in such a way as to
              naturally limit exposure if any particular key is lost or
              compromised. Or forgotten.
             - could involve their bank holding keys, or escrow agents
             - or n-out-of-m voting systems
           - Contracts are the essence...what contracts do people
              voluntarily enter into?
           - And locality--who better to keep keys secure than the
              owner? Anything that transfers blame to "the banks" or to
              "society" breaks the feedback loop of responsibility,
              provides an "out" for the lazy, and encourages fraud
              (people who disavow contracts by claiming their key was
              stolen).
