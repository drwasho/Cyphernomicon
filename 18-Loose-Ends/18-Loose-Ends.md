18. Loose Ends and Miscellaneous Topics
 
 18.1. copyright
            THE  CYPHERNOMICON: Cypherpunks FAQ and More, Version 0.666,
            1994-09-10, Copyright Timothy C. May. All rights reserved.
            See the detailed disclaimer. Use short sections under "fair
            use" provisions, with appropriate credit, but don't put your
            name on my words.
 
 18.2. SUMMARY: Loose Ends and Miscellaneous Topics
   18.2.1. Main Points
   18.2.2. Connections to Other Sections
   18.2.3. Where to Find Additional Information
   18.2.4. Miscellaneous Comments
           - I hate to have a section like this, but there are just some
              things that don't seem to fit neatly elsewhere
           - hopefully you found this topics with your editor search
              tools
 
 18.3. Quantum Cryptography
   18.3.1. "What is quantum cryptography?"
           + Two main flavors:
             + secure channels exploiting the Uncertainty Principle
               + Brassard, Bennett, fiber optic lines, short distances,
                  detects tapping
                 + Quantum cryptography
                   - bits can be exchanged-albeit at fairly low
                      efficiencies-over a channel
                   - with detection of taps, via the change of
                      polarizations
                   + Stephen Wiesner wrote a 1970 paper, half a decade
                      before the P-K work, which outlined this-not
                      published until much later
                     - speculate that the NSA knew about this and
                        quashed the publication
             + factoring of numbers using a strange Many World
                interpretation
               - Shor
               + hearkens to my spoof about Russians
                 - I never knew I hit so close to the mark!
   18.3.2. "What about _quantum cryptography_?"
           + Exploiting Uncertainty Principle to make untappable
              communication lines. (More precisely, tapped lines give
              indication of having been tapped.)
             - Bennett and Brassard
             - faint flashes of light in a fiber optic cable used;
                polarized photons
             - Alice and  Bob go through a protocol that involves them
                picking Linear or Circular Polarization (LP or CP); can't
                be simultaneously measured...
             -
           - Not likely to be important for a long time.
           - An additional tool, or crypto primitive building block.
 
 18.4. Chaotic Cryptography
   18.4.1. the oscillator scheme was broken at Crypto '94
 
 18.5. Neural Nets and AI in Crypto
   18.5.1. "What about neural nets and AI in crypto?"
           - Of limited use, at least in breaking modern ciphers. Marvin
              Minsky once said that if you don't understand how to solve
              a problem, adding randomness usually doesn't help.
           - The shape of  the solution space is very spiky, very poorly-
              suited to hill-climbing or divide-and-conquer methods
           + Neural nets are not likely to do well with modern ciphers
              (e.g., RSA, IDEA, DES, etc.), mainly because of the shape
              of the solution space.  Instead of the "rolling hills and
              valleys" that neural nets (and related methods, such as
              genetic algorithms, simulated annealing, etc.) do well in,
              the solution space for modern ciphers offers very little in
              the way of "learning" opportunities: you either have the
              solution (the key), or you don't.
              
              Think of a needle standing up from a flat plain...a NN or
              any other hill-climber could wander for years and never
              find it. Well-designed modern ciphers like RSA and IDEA
              appear to admit no analysis based on "nonrandom"
              properties. If anybody has found shortcuts to factoring the
              modulus in RSA, for example, they haven't let on.
              
              I suspect there are uses in peripheral aspects, such as
              guessing passwords (when people have not picked high-
              entropy passwords, but have instead used familiar names).
              Or in traffic analysis. Those who munch on lots of traffic
              may well be using neural nets, custom signal processing,
              etc. to "prepare" the captured traffic for further
              analysis. A safe bet, in fact.
              
              But the move in modern cryptology is definitely away from
              using anything with "structure" that can be learned. Put
              another way, neural nets and such work well in structured
              environments, where there's something to _learn), but not
              in the high-entropy, seemingly random world of encrypted
              data.
             + AI may be useful in other areas
               - protocol generation
               - SIGINT
   18.5.2. Evolutionary or Genetic Programming
           - a la Holland, Koza
           - RNGs
 
 18.6. Miscellaneous Advanced Crypto Ideas
   18.6.1. "Why have provably "NP-complete" problems not found uses in
            crypto?"
           - One of the great Unresolved Mysteries! Or the Holy Grail,
              if you will.
           - The issue is why have provably hard (or NP-complete, to be
              more accurate) problems not been used? (Factoring is not
              known to NP-complete...experts can correct my phrasing here
              if I'm misstating things.)
           - It would be nice if a provably hard problem, such as the
              domino tiling problem, or 3SAT, or other such things out of
              Garey and Johnson's book on NP-Completeness could be used.
              This would increase confidence in ciphers still further.
   18.6.2. "Can cellular automata, like Conway's "Game of Life," be used
            for cryptography?"
           - Stephen Wolfram proposed use of cellular automata for
              crytography some years back; his collection of essays on
              cellular automata contains at least one such mention. Many
              people suspected that 1D CAs were no stronger than linear
              feedback shift registers (LFSRs), and I recally hearing a
              couple of years ago that someone proved 1D CAs (and maybe
              all CAs?) are equivalent to LFSRs, which have been used in
              crypto for many years.
           - Wolfram's book is "Theory and Applications of Cellular
              Automata," 1986, World Scientific. Several papers on using
              CAs for random sequence generation. P. Bardell showed
              in1990 that CAs produce the outputs of LFSRs.) Wolfram also
              has a paper, "Cryptography with cellular automata," in
              Proc. CRYPTO 85.
           - Intuitively, the idea of a CA looks attractive for "one-way
              functions," for the reasons mentioned. But what's the
              "trapdoor" that gives the key holder a shortcut to reverse
              the process? (Public key crypto needs a trapdoor 1-way
              funtion that is easy to reverse if one has the right
              information).
 
 18.7. Viruses and Crypto
   18.7.1. "What's the connection between Cypherpunks and viruses?"
           - Like, dewd, it's so kool.
           - Beavis 'n Butthead use PGP (actually, Eric Hughes proposed
              at one point that we suggest a crypto tie-in to the
              writers)
           - There's only peripheral connection.
           - Viruses can be spread with anonymous remailers, but digital
              signatures can be used to safeguard software. Signed
              software, no mods allowed.
   18.7.2. "What about the "encryption viruses," like KOH?"
           - (A little far afield, but the issue does come up.)
           - Somebody asked about this on sci.crypt and Vesselin
              Bontchev said:  "This topic has been debated to death in
              alt.security.pgp, when somebody posted KOH, without even a
              warning that it is a virus.....Both viruses indeed use the
              IDEA cipher - the same that is used both by SecureDevice
              and SecureDrive. However, the viruses pose some significant
              threats to the integrity of your data, exactly because of
              their viral replication means.....Also, if you aquire it by
              viral means, you do not get the doumentation and one
              utility, both of which are essential for the proper usage
              of the product - thus proving one more time that its viral
              capabilities are unnecessary and harmful. Also, the virus
              does not come in source, which means that it could have
              some hidden backdoors or simply security flaws, and you
              have no way to check this or to fix them. At last, in some
              cases the virus could destroy valuable information during
              its replication process."
           - "In short - don't use them. You will gain nothing over
              using
              stand-alone encryption programs, and you'll expose your
              data's
              integrity to significant risks. Those viruses are
              completely useless
              and even harmful; they have been created with the only
              reason to
              condone the illicit activities of the virus writers, by
              claiming that
              computer viruses can be "useful"." [Vesselin Bontchev,
              sci.crypt, 1994-08-31]
   18.7.3. "What about viruses? Are there any ties to crypto and
            Cypherpunks themes?"
           - No direct link that any of us see clearly. Occasionally a
              virus fan sees the "punks" name and thinks we're involved
              in writing viruses. (Actually, a few folks on the list have
              virus expertise.)
           - Crypto may protect against viruses, by having code signed.
              And the reliance on self-responsibility and self-protection
              is in contrast to the legal approach, which tends not to
              work too well for virus protection (by the covert nature of
              many viruses).
   18.7.4. "What interests do Cypherpunks have in viruses?"
           - Not much, though the topic comes up periodically.
           - Some overlap in the communities involved.
           - And there are some virus methods which use forms of
              encryption.
           - Also, digital signatures on code can be used to ensure that
              code has not been modified since being released by the
              original author.
 
 18.8. Making Money in Crypto
   18.8.1. "How can I make money in crypto?"
           - crypto experts are hired by software companies
           + start up companies
             - a tough road
             - not clear that even Phil Zimmermann has made money
             - and even RSADSI is facing a challenge (hasn't gone
                public, not a cash cow, etc.)
           - There may be an explosive growth--the phase change I often
              talk about--and many opportunities will emerge. But, having
              said this, I still don't see obvious opportunities right
              now. And starting a company based on hope and ideology,
              rather than supplying a real market or pushing real
              technology (market pull vs. technology push argument) seem
              misguided.
 
 18.9. The Net
   18.9.1. Limitations of the current net
           - interoperability
           + subsidized, not pay as you go
             - makes spamming inevitable, doesn't allocate resources to
                those who want them the most
             - this will require digicash in a better form than most
                users now have access to
           - sysadmins get worried
           - encryption sometimes banned
           - common carrier status not clear
           - general cruftiness of Net ("imminent death of Usenet
              predicted")

18.10. Duress Switches, Dead Man Switches
  18.10.1. "What about "duress" codes for additional security?"
           - Where a harmless decrytion can be done, or an alarm sent.
           + Examples
             - sending alarm, like an under the counter alarm button
             - decrypting a bank card number for a lesser-value account
             - two sets of books (not strictly a "duress" code, unless
                you view the IRS as causing duress)
             - alarms to associates, as in cells
           - " Having a separate authentication mechanism that is used
              under duress is a very good idea that some existing systems
              already
              employ....  From a systems point of view, it is hard to
              figure out exactly how the system should respond when it
              recognizes a duress authentication....The safe inside the
              ATM machines used by BayBanks (Boston Mass) can be opened
              with two combinations.  One combination sends an alarm to
              the bank via a separate phone line (not the one used to
              perform the ATM transaction).  The alarm phone line is also
              connected to a conventional panic switch." [Bob Baldwin,
              Duress Passwords/PINs/Combinations, 1993-11-18]
  18.10.2. Duress switches, dead man switches, etc.
           + "Digital flash paper," can be triggered to erase files,
              etc.
             - (BATF and DEA raiders may have sophisticated means of
                disabling computers)
           + Duress codes..."erase my files," ways of not giving esrowed
              information unless proper code is given, etc.
             + "Don't release if I am under indictment"
               - interesting issues about secret indictments, about
                  publicity of such cases, access to court records by
                  offshore computers, etc.
  18.10.3. Personal security for disks, dead man switches
           + I have heard that some BBS operators install dead man
              switches near the doors to rooms containing their
              systems...entering the room without flipping the switch
              causes some action to be taken
             - erasing a disk, dumping a RAM disk (a dangerous way to
                store data, given power failures, soft errors, restarts,
                etc.)

18.11. Can Encryption be Detected?
  18.11.1. "Can messages be scanned and checked for encryption?"
           - If the encryption produces _markers_ or other indications,
              then of course. "BEGIN PGP" is a pretty clear beacon. (Such
              markers assists in decryption by the recipient, but are not
              essential. "Stealth" versions of PGP and other encryption
              programs--such as S-Tools for DOS--don't have such
              markers.)
           - If the encryption produces "random-looking" stuff, then
              entropy measures and other statistical tests may or may not
              be able detect such messages reliably. Depends on what non-
              encrypted messages look like, and how the algorithm  works.
           + Steganography:
             - making messages look like normal ones
             - tucking th ebits in with other random-like bits, such as
                in the low-order bits of images or sound files
           - The practical concern depends on one's local political
              environment. In many countries, mere suspicion of using
              crypto could put one in real danger.

18.12. Personal Digital Assistants, Newtons, etc.
  18.12.1. "Are there cryptographic uses for things like Newtons?"
           - Probably. Eventually. Digital wallets, portable key
              holders, local agents for access, etc.
           + Meanwhile, a few encryption programs exist. Here's one:
             - -> nCrypt, the strong cryptography application for
                Newton:
                -> ftp.sumex-aim.stanford.edu/info-mac/nwt/utils/n-crypt-
                lite.hqx

18.13. Physical Security
  18.13.1. "Can fiber optical cables be tapped?"
           + Yes. Light can escape from the fiber in bends, and "near-
              field" tapping is theoretically possible, at least under
              lab conditions. Active measures for puncturing cable
              shields and tapping fibers are also possible.
             - "The Fed's want a cost effective F/O tap. My company was
                approached to develop such a system, can be done but not
                cheap like copper wire tapping." [
                domonkos@access.digex.net (andy domonkos),
                comp.org.eff.talk, 1994-06-29]
           - Los Alamos technology? 1990?

18.14. Attacking Governments
  18.14.1. "termites" (rumors, psy-ops) that can undermine governments,
            followed by "torpedoes" (direct attack)
  18.14.2. WASTE (War Against Strong, Tamper-resistant Encryption).

18.15. Cypherpunks List Issues
  18.15.1. too much noise on the list?
           - "Of all the lists I'm subscribed to, this is the only one
              that I read
              *every* article in.  Even the "noise" articles.  Humans
              being what
              they are, the noise is needed to help decide the direction
              of the
              group.  Besides, for those of us who are just starting on
              our journey
              through crypto-underworld need the noise to help
              familiarize
              ourselves with how crypto works.  I've learned more from
              the informal
              ramblings than I've gathered out of all the formal and/or
              mathematical
              postings to date." [Patrick E. Hykkonen, 5-25-93]

18.16. Tamper-Resistant Modules
  18.16.1. TRMs--claims that "Picbuster" processor can be locally
            overwritten with focussed or directed UV (OTP)
  18.16.2. tamper-resistant modules have some downsides as well
           - cash registers for ensuring compliance with all relevant
              sales tax, value-added tax (VAT), and rationing rules; a
              tamper-resistant module cash register could be the
              enforcement mechanism for a national security state.
           - "observers"

18.17. Deeper Connections
  18.17.1. In several places I've referred to "deep connections" between
            things like crypto, money, game theory, evolutionary
            ecologies, human motivations, and the nature of law. By this
            I mean that there are deeper, unifying principles. Principles
            involving locality, identity, and disclosure of knowledge. A
            good example: the deep fairness of "cut-and-choose" protocols-
            -I've seen mention of this in game theory tesxts, but not
            much discussion of other, similar protocols.
  18.17.2. For example, below the level of number theory and algorithms
            in cryptology lies a level dealing with "identity," "proof,"
            "collusion," and other such core concepts, concepts that can
            almost be dealt with independent of the acual algorithms
            (though the concrete realization of public key methods took
            this out of the abstract realm of philosophy and made it
            important to analyze). And these abstract concepts are linked
            to other fields, such as economics, human psychology, law,
            and evolutionary game theory (the study of evolved strategies
            in multi-agent systems, e.g., human beings interacting and
            trading with each other).
  18.17.3. I believe there are important questions about why things work
            the way they do at this level. To be concrete, why do threats
            of physical coercion create market distortions and what
            effects does this have? Or, what is the nature of emergent
            behavior in reputation-based systems? (The combinatiion of
            crypto and economics is a fertile area, barely touched upon
            by the academic cryptology community.) Why is locality is
            important, and what does this mean for digital cash? Why does
            regulation often produce _more_ crime?
  18.17.4. Crypto and the related ideas of reputation, identity, and
            webs of trust has introduced a new angle into economic
            matters. I suspect there are a couple of Nobel Prizes in
            Economics for those who integrate these important concepts.

18.18. Loose End Loose Ends
  18.18.1. What the core issues are...a tough thing to analyze
           - untraceablility as a basic construct has major implications
           + can often ask what the implications would be if, say:
             - invisibility existed
             - untraceability existed
           - By "tough to analyze" I mean that things are often
              coflated, mixed together. Is it the "reputations" that
              matter, or the "anonymity"? The "untraceability" or the
              "digital money"?
  18.18.2. Price signalling in posts...for further information
           + When an article is posted, and there is more complete
              information available elsewhere by ftp, gopher, mosaic,
              etc., then how is this to to be signalled without actually
              advertising prominently?
             - why not a code, like the "Geek code" so many people put
                in their sigs? The code could be parsed by a reader and
                used to automatically fetch the information, pay for it,
                etc. (Agents that can be built in to newsreaders.)
  18.18.3. "What should Cypherpunks support for "cable" or "set-top box"
            standards?
           - Caveats: My opinions, offered only to help frame the
              debate. And many of us reject the idea of government-
              mandated "standards," so my phrasing here is not meant to
              imply support of such standards.
           + Major alternatives:
             + Set-top box, with t.v. as core of access to "information
                superhighway."
               + Problems:
                 - limited number of channels, even if "500 channels"
                 - makes t.v. the focus, loses some other capabilities
                 - few consumers will have television sets with the
                    resolution capabilities that even current computer
                    monitors have (there are reasons for this: size of
                    monitors (related to viewing distance), NTSC
                    constraints, age of televisions, etc.)
             + Switched-packet cable, as in ATM or even SONET
                (Synchronous Optical Network) access
               + Advantages:
                 - Television is just one more switched-packet
                    transmission, not using up the bandwidth
             + Radical Proposal: Complete deregulation
               + let cable suppliers--especially of optical fibers,
                  which are small and unobtrusive--lay fibers to any home
                  they can negotiate access to
                 - e.g., by piggybacking on telephone lines, electrical
                    cables, etc. (to remove the objection about unsightly
                    new poles or cables being strung...should not be an
                    issue with fiber optics)
               - let the market decide...let customers decide
           + In my view, government standards are a terrible idea here.
              Sure, NTSC was an effective standard, but it likely would
              have emerged without government involvement. Ditto for
              Ethernet and a zillion other standards. No need for
              government involvement.
             - Of course, when industry groups meet to discuss
                standards, one hopes that antitrust laws will not be
                invoked.
  18.18.4. minor point: the importance of "But does it scale?" is often
            exaggerated
           - in many cases, it's much more important to simply get
              something deployed than it is to worry in advance about how
              it will break if too many people use it (e.g., MacDonald's
              worrying in 1955 about scalabilty of their business).
           - Remailer networks, for example, may not scale especially
              well in their current form...but who cares? Getting them
              used will allow further refinement.
