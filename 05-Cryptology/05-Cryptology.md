5. Cryptology
  
  5.1. copyright
            THE  CYPHERNOMICON: Cypherpunks FAQ and More, Version 0.666,
            1994-09-10, Copyright Timothy C. May. All rights reserved.
            See the detailed disclaimer. Use short sections under "fair
            use" provisions, with appropriate credit, but don't put your
            name on my words.
  
  5.2. SUMMARY: Cryptology
    5.2.1. Main Points
           - gaps still exist here...I treated this as fairly low
              priority, given the wealth of material on cryptography
    5.2.2. Connections to Other Sections
           - detailed crypto knowledge is not needed to understand many
              of the implications, but it helps to know the basics (it
              heads off many of the most wrong-headed interpretations)
           - in particular, everyone should learn enough to at least
              vaguely understand how "blinding" works
    5.2.3. Where to Find Additional Information
           + a dozen or so major books
             - Schneier, "Applied Cryptography"--is practically
                "required reading"
             - Denning
             - Brassard
             - Simmons
             - Welsh, Dominic
             - Salomaa
             - "CRYPTO" Proceedings
             - Other books I can take or leave
           - many ftp sites, detailed in various places in this doc
           - sci.crypt, alt.privacy.pgp, etc.
           - sci.crypt.research is a new group, and is moderated, so it
              should have some high-quality, technical posts
           - FAQs on sci.crypt, from RSA, etc.
           - Dave Banisar of EPIC (Electronic Privacy Information
              Center) reports: "...we have several hundred files on
              encryption available via ftp/wais/gopher/WWW from cpsr.org
              /cpsr/privacy/crypto." [D.B., sci.crypt, 1994-06-30]
    5.2.4. Miscellaneous Comments
           - details of algorithms would fill several books...and do
           - hence, will not cover crypto in depth here (the main focus
              of this doc is the implications of crypto, the
              Cypherpunkian aspects, the things not covered in crypto
              textbooks)
           - beware of getting lost in the minutiae, in the details of
              specific algorithms...try to keep in the mind the
              _important_ aspects of any system
  
  5.3. What this FAQ Section Will Not Cover
    5.3.1. Why a section on crypto when so many other sources exist?
           - A good question. I'll be keeping this section brief, as
              many textbooks can afford to do a much better job here than
              I can.
           - not just for those who read number theory books with one
              hand
    5.3.2. NOTE: This section may remain disorganized, at least as
            compared to some of the later sections. Many excellent
            sources on crypto exist, including readily available FAQs
            (sci.crypt, RSADSI FAQ) and books. Schneier's books is
            especially recommended, and should be on _every_ Cypherpunk's
            bookshelf.
  
  5.4. Crypto Basics
    5.4.1. "What is cryptology?"
           - we see crypto all around us...the keys in our pockets, the
              signatures on our driver's licenses and other cards, the
              photo IDs, the credit cards
           + cryptography or cryptology, the science of secret
              writing...but it's a lot more...consider I.D.  cards, locks
              on doors, combinations to safes, private
              information...secrecy is all around us
             - some say this is bad--the tension between "what have you
                got to hide?" and "none of your business"
           - some exotic stuff: digital money, voting systems, advanced
              software protocols
           - of importance to protecting privacy in a world of
              localizers (a la Bob and Cherie), credit cards, tags on
              cars, etc....the dossier society
           + general comments on cryptography
             - chain is only as strong as its weakest link
             - assume opponnent knows everything except the secret key
             -
           - Crypto is about economics
           + Codes and Ciphers
             + Simple Codes
               - Code Books
             + Simple Ciphers
               + Substitution Ciphers (A=C, B=D, etc.)
                 - Caesar Shift (blocks)
               + Keyword Ciphers
                 + Vigenre (with Caesar)
                   + Rotor Machines
                     - Hagelin
                     - Enigma
                     - Early Computers (Turing, Colossus)
             + Modern Ciphers
               + 20th Century
                 + Private Key
                   + One-Time Pads (long strings of random numbers,
                      shared by both parties)
                     + not breakable even in principle, e.g., a one-time
                        pad with random characters selected by a truly
                        random process (die tosses, radioactive decay,
                        certain types of noise, etc.)
                       - and ignoring the "breakable by break-ins"
                          approach of stealing the one-time pad, etc.
                          ("Black bag cryptography")
                     - Computer Media (Floppies)
                     + CD-ROMs and DATs
                       - "CD ROM is a terrible medium for the OTP key
                          stream.  First, you want exactly two copies of
                          the random stream.  CD ROM has an economic
                          advantage only for large runs. Second, you want
                          to destroy the part of the stream already used.
                          CD ROM has no erase facilities, outside of
                          physical destruction of the entire disk."
                          [Bryan G. Olson, sci.crypt, 1994-08-31]
                   + DES--Data Encryption Standard
                     - Developed from IBM's Lucifer, supported by NSA
                     - a standard since 1970s
                     + But is it "Weak"?
                       + DES-busting hardware and software studied
                         + By 1990, still cracked
                           - But NSA/NIST has ordered a change
                   + Key Distribution Problem
                     + Communicating with 100 other people means
                        distributing and  securing 100 keys
                       - and each of those 100 must keep their 100 keys
                          secure
                       - no possibility of widespread use
                 + Public Key
                   + 1970s: Diffie, Hellman, Merkle
                     + Two Keys: Private Key and Public Key
                       + Anybody can encrypt a message to Receiver with
                          Receiver's PUBLIC key, but only the Receiver's
                          PRIVATE key can decrypt the message
                         + Directories of public keys can be published
                            (solves the key distribution problem)
                           + Approaches
                             + One-Way Functions
                               - Knapsack (Merkle, Hellman)
                               + RSA (Rivest, Shamir, Adleman)
                                 - relies on difficulty of factoring
                                    large numbers (200 decimal digits)
                                 - believed to be "NP-hard"
                                 + patented and licensed to "carefully
                                    selected" customers
                                   - RSA, Fiat-Shamir, and other
                                      algorithms are not freely usable
                                   - search for alternatives continues
    5.4.2. "Why does anybody need crypto?"
           + Why the Need
             - electronic communications...cellular phones, fax
                machines, ordinary phone calls are all easily
                intercepted...by foreign governments, by the NSA, by
                rival drug dealers, by casual amateurs
             + transactions being traced....credit card receipts,
                personal checks, I.D. cards presented at time of
                purchase...allows cross-referencing, direct mail data
                bases, even government raids on people who buy greenhouse
                supplies!
               - in a sense, encryption and digital money allows a
                  return to cash
             - Why do honest people need encryption? Because not
                everyone is honest, and this applies to governments as
                well. Besides, some things are no one else's  business.
           - Why does anybody need locks on doors? Why aren't all
              diaries available for public reading?
           + Whit Diffie, one of the inventors of public key
              cryptography (and a Cypherpunk) points out that human
              interaction has largely been predicated on two important
              aspects:
             - that you are who you say you are
             - expectation of privacy in private communications
           - Privacy exists in various forms in various cultures. But
              even in police states, certain concepts of privacy are
              important.
           - Trust is not enough...one may have opponents who will
              violate trust if it seems justified
           + The current importance of crypto is even more striking
             + needed to protect privacy in cyberspace, networks, etc.
               - many more paths, links, interconnects
               - read Vinge's "True Names" for a vision
             + digital money...in a world of agents, knowbots, high
                connectivity
               - (can't be giving out your VISA number for all these
                  things)
             + developing battle between:
               - privacy advocates...those who want privacy
               - government agencies...FBI, DOJ, DEA, FINCEN, NSA
               + being fought with:
                 - attempts to restrict encryption (S.266, never passed)
                 - Digital Telephony Bill, $10K a day fine
                 - trial balloons to require key registration
                 - future actions
           + honest people need crypto because there are dishonest
              people
             - and there may be other needs for privacy
           - Phil Zimmerman's point about sending all mail, all letters,
              on postcards--"What have you got to hide?" indeed!
           - the expectation of privacy in out homes and in phone
              conversations
           + Whit Diffie's main points:
             + proving who you say you are...signatures, authentications
               - like "seals" of the past
             - protecting privacy
             - locks and keys on property and whatnot
           + the three elements that are central to our modern view of
              liberty and privacy (a la Diffie)
             - protecting things against theft
             - proving who we say we are
             - expecting privacy in our conversations and writings
    5.4.3. What's the history of cryptology?
    5.4.4. Major Classes of Crypto
           - (these sections will introduce the terms in context, though
              complete definitions will not be given)
           + Encryption
             - privacy of messages
             - using ciphers and codes to protect the secrecy of
                messages
             - DES is the most common symmetric cipher (same key for
                encryption and decryption)
             - RSA is the most common asymmetric cipher (different keys
                for encryption and decryption)
           + Signatures and Authentication
             - proving who you are
             - proving you signed a document (and not someone else)
             + Authentication
               + Seals
                 + Signatures (written)
                   + Digital Signatures (computer)
                     - Example: Numerical codes on lottery tickets
                     + Using Public Key Methods (see below)
                       - Digital Credentials (Super Smartcards)
                 - Tamper-responding Systems
               + Credentials
                 - ID Cards, Passports, etc.
               + Biometric Security
                 - Fingerprints, Retinal Scans, DNA, etc.
           + Untraceable Mail
             - untraceable sending and receiving of mail and messages
             - focus: defeating eavesdroppers and traffic analysis
             - DC protocol (dining cryptographers)
           + Cryptographic Voting
             - focus: ballot box anonymity
             - credentials for voting
             - issues of double voting, security, robustness, efficiency
           + Digital Cash
             - focus: privacy in transactions, purchases
             - unlinkable credentials
             - blinded notes
             - "digital coins" may not be possible
           + Crypto Anarchy
             - using the above to evade gov't., to bypass tax
                collection, etc.
             - a technological solution to the problem of too much
                government
           + Security
             + Locks
               - Key Locks
               + Combination Locks
                 - Cardkey Locks
             + Tamper-responding Systems (Seals)
               + Also known as "tamper-proof" (misleading)
                 - Food and Medicine Containers
                 - Vaults, Safes (Alarms)
                 + Weapons, Permissive Action Links
                   - Nuclear Weapons
                   - Arms Control
                 - Smartcards
                 - Currency, Checks
                 + Cryptographic Checksums on Software
                   - But where is it stored? (Can spoof the system by
                      replacing the whole package)
                 + Copy Protection
                   - Passwords
                   - Hardware Keys ("dongles")
                   - Call-in at run-time
             + Access Control
               - Passwords, Passphrases
               - Biometric Security, Handwritten Signatures
               - For: Computer Accounts, ATMs, Smartcards
    5.4.5. Hardware vs. Software
           - NSA says only hardware implementations can really be
              considered secure, and yet most Cypherpunks and ordinary
              crypto users favor the sofware approach
           - Hardware is less easily spoofable (replacement of modules)
           - Software can be changed more rapidly, to make use of newer
              features, faster modules, etc.
           - Different cultures, with ordinary users (many millions)
              knowing they are less likely to have their systems black-
              bag spoofed (midnight engineering) than are the relatively
              fewer and much more sensitive military sites.
    5.4.6. "What are 'tamper-resistant modules' and why are they
            important?"
           - These are the "tamper-proof boxes" of yore: display cases,
              vaults, museum cases
           - that give evidence of having been opened, tampered with,
              etc.
           + modern versions:
             - display cases
             - smart cards
             + chips
               - layers of epoxy, abrasive materials, fusible links,
                  etc.
               - (goal is to make reverse engineering much more
                  expensive)
             - nuclear weapon "permissive action links" (PALs)
    5.4.7. "What are "one way functions"?"
           - functions with no inverses
           - crypto needs functions that are seemingly one-way, but
              which actually have an inverse (though very hard to find,
              for example)
           - one-way function, like "bobbles" (Vinge's "Marooned in
              Realtime")
    5.4.8. When did modern cryptology start?
           + "What are some of the modern applications of cryptology?"
             + "Zero Knowledge Interactive Proof Systems" (ZKIPS)
               - since around 1985
               - "minimum disclosure proofs"
               + proving that you know something without actually
                  revealing that something
                 + practical example: password
                   + can prove you have the password without actually
                      typing it in to computer
                     - hence, eavesdroppers can't learn your password
                     - like "20 questions" but more sophisticated
                 - abstract example: Hamiltonian circuit of a graph
             + Digital Money
               + David Chaum: "RSA numbers ARE money"
                 - checks, cashiers checks, etc.
                 - can even know if attempt is made to cash same check
                    twice
                 + so far, no direct equivalent of paper currency or
                    coins
                   - but when combined with "reputation-based systems,"
                      there may be
             + Credentials
               + Proofs of some property that do not reveal more than
                  just that property
                 - age, license to drive, voting rights, etc.
                 - "digital envelopes"
               + Fiat-Shamir
                 - passports
             + Anonymous Voting
               - protection of privacy with electronic voting
               - politics, corporations, clubs, etc.
               - peer review of electronic journals
               - consumer opinions, polls
             + Digital Pseudonyms and Untraceable E-Mail
               + ability to adopt a digital pseudonym that is:
                 - unforgeable
                 - authenticatable
                 - untraceable
               - Vinge's "True Names" and Card's "Ender's Game"
               + Bulletin Boards, Samizdats, and Free Speech
                 + banned speech, technologies
                   - e.g., formula for RU-486 pill
                   - bootleg software, legally protected material
                 + floating opinions without fears for professional
                    position
                   - can even later "prove" the opinions were yours
               + "The Labyrinth"
                 - store-and-forward switching nodes
                 + each with tamper-responding modules that decrypt
                    incoming messages
                   + accumulate some number (latency)
                     + retransmit to next address
                       - and so on....
                 + relies on hardware and/or reputations
                   + Chaum claims it can be done solely in software
                     - "Dining Cryptographers"
    5.4.9. What is public key cryptography?
   5.4.10. Why is public key cryptography so important?
           + The chief advantage of public keys cryptosystems over
              conventional symmetric key (one key does both encryption
              and decryption) is one _connectivity_ to recipients: one
              can communicate securely with people without exchanging key
              material.
             - by looking up their public key in a directory
             - by setting up a channel using Diffie-Hellman key exchange
                (for example)
   5.4.11. "Does possession of a key mean possession of *identity*?"
           - If I get your key, am I you?
           - Certainly not outside the context of the cryptographic
              transaction. But within the context of a transaction, yes.
              Additional safeguards/speedbumps can be inserted (such as
              biometric credentials, additional passphrases, etc.), but
              these are essentially part of the "key," so the basic
              answer remains "yes." (There are periodically concerns
              raised about this, citing the dangers of having all
              identity tied to a single credential, or number, or key.
              Well, there are ways to handle this, such as by adopting
              protocols that limit one's exposure, that limits the amount
              of money that can be withdrawn, etc. Or people can adopt
              protocols that require additional security, time delays,
              countersigning, etc.)
           + This may be tested in court soon enough, but the answer for
              many contracts and crypto transactions will be that
              possession of key = possession of identity. Even a court
              test may mean little, for the types of transactions I
              expect to see.
             - That is, in anonymous systems, "who ya gonna sue?"
           - So, guard your key.
   5.4.12. What are digital signatures?
           + Uses of Digital Signatures
             - Electronic Contracts
             - Voting
             - Checks and other financial instruments (similar to
                contracts)
             - Date-stamped Transactions (augmenting Notary Publics)
   5.4.13. Identity, Passports, Fiat-Shamir
           - Murdoch, is-a-person, national ID cards, surveillance
              society
           + "Chess Grandmaster Problem" and other Frauds and Spoofs
             - of central importance to proofs of identity (a la Fiat-
                Shamir)
             - "terrorist" and "Mafia spoof" problems
   5.4.14. Where  else should I look?
   5.4.15. Crypto, Technical
           + Ciphers
             - traditional
             - one-time pads, Vernams ciphers, information-theoretically
                secure
             + "I Have a New Idea for a Cipher---Should I Discuss it
                Here?"
               - Please don't. Ciphers require careful analysis, and
                  should be in paper form (that is, presented in a
                  detailed paper, with the necessary references to show
                  that due diligence was done, the equations, tables,
                  etc. The Net is a poor substitute.
               - Also, breaking a randomly presented cipher is by no
                  means trivial, even if the cipher is eventually shown
                  to be weak. Most people don't have the inclination to
                  try to break a cipher unless there's some incentive,
                  such as fame or money involved.
               - And new ciphers are notoriously hard to design. Experts
                  are the best folks to do this. With all the stuff
                  waiting to be done (described here), working on a new
                  cipher is probably the least effective thing an amateur
                  can do. (If you are not an amateur, and have broken
                  other people's ciphers before, then you know who you
                  are, and these comments don't apply. But I'll guess
                  that fewer than a handful of folks on this list have
                  the necessary background to do cipher design.)
               - There are a vast number of ciphers and systems, nearly
                  all of no lasting significance. Untested, undocumented,
                  unused--and probably unworthy of any real attention.
                  Don't add to the noise.
             - What is DES and can it be broken?
             + ciphers
               - RC4, stream cipher
               + DolphinEncrypt
                 -
                 + "Last time Dolphin Encrypt reared its insecure head
                    in this forum,
                   - these same issues came up.  The cipher that DE uses
                      is not public and
                   - was not designed by a person of known
                      cryptographicc competence.  It
                   - should therefore be considered extremely weak.
                      <Eric Hughes, 4-16-94, Cypherpunks>
           + RSA
             - What is RSA?
             - Who owns or controls the RSA patents?
             - Can RSA be broken?
             - What alternatives to RSA exist?
           + One-Way Functions
             - like diodes, one-way streets
             - multiplying two large numbers together is
                easy....factoring the product is often very hard
             - (this is not enough for a usable cipher, as the recipient
                must be able to perform the reverse operation..it turns
                out that "trapdoors" can be found)
           - Digital Signatures
           + Digital Cash
             - What is digital cash?
             - How does digital cash differ from VISA and similar
                electronic systems?
             - Clearing vs. Doublespending Detection
           - Zero Knowledge
           - Mixes and Remailers
           - Dining Cryptographers
           + Steganography
             - invisible ink
             - microdots
             - images
             - sound files
           + Random Number Generators
             + von Neumann quote about living in a state of sin
               - also paraphrased (I've heard) to include _analog_
                  methods, presumably because the nonrepeating (form an
                  initial seed/start)  nature makes repeating experiments
                  impossible
             + Blum-Blum-Shub
               + How it Works
                 - "The Blum-Blum-Shub PRNG is really very simple.
                    There is source floating around on the crypto ftp
                    sites, but it is a set of scripts for the Unix bignum
                    calculator "bc", plus some shell scripts, so it is
                    not very portable.
                    
                    "To create a BBS RNG, choose two random primes p and
                    q which are congruent to 3 mod 4.  Then the RNG is
                    based on the iteration x = x*x mod n.  x is
                    initialized as a random seed.  (x should be a
                    quadratic residue, meaning that it is the square of
                    some number mod n, but that can be arranged by
                    iterating the RNG once before using its output.)"
                    [Hal Finney, 1994-05-14]
               - Look for blum-blum-shub-strong-randgen.shar and related
                  files in pub/crypt/other at ripem.msu.edu. (This site
                  is chock-full of good stuff. Of course, only Americans
                  are allowed to use these random number generators, and
                  even they face fines of $500,000 and imprisonment for
                  up to 5 years for inappopriate use of random numbers.)
               - source code at ripem ftp site
               - "If you don't need high-bandwidth randomness, there are
                  several good PRNG, but none of them run fast.  See the
                  chapter on PRNG's in "Cryptology and Computational
                  Number Theory"." [Eric Hughes, 1994-04-14]
             + "What about hardware random number generators?"
               + Chips are available
                 -
                 + "Hughes Aircraft also offers a true non-deterministic
                    chip (16 pin DIP).
                   - For more info contact me at kephart@sirena.hac.com"
                      <7 April 94, sci.crypt>
             + "Should RNG hardware be a Cypherpunks project?"
               - Probably not, but go right ahead. Half a dozen folks
                  have gotten all fired up about this, proposed a project-
                  -then let it drop.
             - can use repeated applications of a cryptographic has
                function to generate pretty damn good PRNs (the RSAREF
                library has hooks for this)
             + "I need a pretty good random number generator--what
                should I use?"
               - "While Blum-Blum-Shub is probably the cool way to go,
                  RSAREF uses repeated iterations of MD5 to generate its
                  pseudo-randoms, which can be reasonably secure and use
                  code you've probably already got hooks from perl
                  for.[BillStewart,1994-04-15]
             + Libraries
               - Scheme code: ftp://ftp.cs.indiana.edu/pub/scheme-
                  repository/scm/rand.scm
           + P and NP and all that jazz
             - complexity, factoring,
             + can quantum mechanics help?
               - probably not
           + Certification Authorities
             - heierarchy vs. distributed web of trust
             - in heierarchy, individual businesses may set themselves
                up as CAs, as CommerceNet is talking about doing
             + Or, scarily, the governments of the world may insist that
                they be "in the loop"
               - several ways to do this: legal system invocation, tax
                  laws, national security....I expect the legal system to
                  impinge on CAs and hence be the main way that CAs are
                  partnered with the government
               - I mention this to give people some chance to plan
                  alternatives, end-runs
             - This is one of the strongest reasons to support the
                decoupling of software from use (that is, to reject the
                particular model RSADSI is now using)
   5.4.16. Randomness
           - A confusing subject to many, but also a glorious subject
              (ripe with algorithms, with deep theory, and readily
              understandable results).
           + Bill Stewart had a funny comment in sci.crypt which also
              shows how hard it is to know if something's really random
              or not: "I can take a simple generator X[i] = DES( X[i-1],
              K ), which will produce nice random white noise, but you
              won't be able to see that it's non-random unless you rent
              time on NSA's DES-cracker." [B.S. 1994-09-06]
             - In fact, many seemingly random strings are actually
                "cryptoregular": they are regular, or nonrandom, as soon
                as one uses the right key. Obviously, most strings used
                in crypto are cryptoregular in that they _appear_ to be
                random, and pass various randomness measures, but are
                not.
           + "How can the randomness of a bit string be measured?"
             - It can roughly be estimated by entropy measures, how
                compressible it is (by various compression programs),
                etc.
             - It's important to realize that measures of randomness
                are, in a sense, "in the eye of the beholder"--there just
                is no proof that a string is random...there's always room
                for cleverness, if you will
             + Chaitin-Kolmogoroff complexity theory makes this clearer.
                To use someone else's words:
               - "Actually, it can't be done.  The consistent measure of
                  entropy for finite objects like a string or a (finite)
                  series of random numbers is the so-called ``program
                  length complexity''.  This is defined as the length of
                  the shortest program for some given universal Turing
                  machine
                  which computes the string.  It's consistent in the
                  sense that it has the familiar properties of
                  ``ordinary'' (Shannon) entropy.  Unfortunately, it's
                  uncomputable: there's no algorithm which, given an
                  arbitrary finite string S, computes the program-length
                  complexity of S.
                  
                  Program-length complexity is well-studied in the
                  literature.  A good introductory paper is ``A Theory of
                  Program Size Formally Identical to Information Theory''
                  by  G. J. Chaitin, _Journal of the ACM_, 22 (1975)
                  reprinted in Chaitin's book _Information Randomness &
                  Incompleteness_, World Scientific Publishing Co.,
                  1990." [John E. Kreznar, 1993-12-02]
           + "How can I generate reasonably random numbers?"
             - I say "reasonably" becuae of the point above: no number
                or sequence is provably "random." About the best that can
                be said is that a number of string is the reuslt of a
                process we call "random." If done algorithimically, and
                deterministically, we call this process "pseudo-random."
                (And  pseudorandom is usually more valuable than "really
                random" because we want to be able to generate the same
                sequence repeatedly, to repeat experiments, etc.)
   5.4.17. Other crypto and hash programs
           + MDC, a stream cipher
             - Peter Gutman, based on NIST Secure Hash Algorithm
             - uses longer keys than IDEA, DES
           - MD5
           - Blowfish
           - DolphinEncrypt
   5.4.18. RSA strength
           - casual grade, 384 bits, 100 MIPS-years (Paul Leyland, 3-31-
              94)
           - RSA-129, 425 bits, 4000 MIPS-years
           - 512 bits...20,000 MIPS-years
           - 1024 bits...
   5.4.19. Triple DES
           - "It involves three DES cycles, in encrypt-decrypt-encrypt
              order. THe keys used may be either K1/K2/K3 or K1/K2/K1.
              The latter is   sometimes caled "double-DES".  Combining
              two DES operations like this requires twice as much work to
              break as one DES, and a lot more storage. If you have the
              storage, it just adds one bit to the effective key size.  "
              [Colin Plumb, colin@nyx10.cs.du.edu, sci.crypt, 4-13-94]
   5.4.20. Tamper-resistant modules (TRMs) (or tamper-responding)
           + usually "tamper-indicating", a la seals
             - very tough to stop tampering, but relatively easy to see
                if seal has been breached (and then not restored
                faithfully)
             - possession of the "seal" is controlled...this is the
                historical equivalent to the "private key" in a digital
                signature system, with the technological difficulty of
                forging the seal being the protection
           + usually for crypto. keys and crypto. processing
             - nuclear test monitoring
             - smart cards
             - ATMs
           + one or more sensors to detect intrusion
             - vibration (carborundum particles)
             - pressure changes (a la museum display cases)
             - electrical
             - stressed-glass (Corning, Sandia)
           + test ban treaty verification requires this
             - fiber optic lines sealing a missile...
             - scratch patterns...
             - decals....
           + Epoxy resins
             - a la Intel in 1970s (8086)
             + Lawrence Livermore: "Connoisseur Project"
               - gov't agencies using this to protect against reverse
                  engineering, acquisition of keys, etc.
             + can't stop a determined effort, though
               - etches, solvents, plasma ashing, etc.
               - but can cause cost to be very high (esp. if resin
                  formula is varied frequently, so that "recipe" can't be
                  logged)
             + can use clear epoxy with "sparkles" in the epoxy and
                careful 2-position photography used to record pattern
               - perhaps with a transparent lid?
           + fiber optic seal (bundle of fibers, cut)
             - bundle of fibers is looped around device, then sealed and
                cut so that about half the fibers are cut; the pattern of
                lit and
                unlit fibers is a signature, and is extremely difficult
                to reproduce
           - nanotechnology may be used (someday)
   5.4.21. "What are smart cards?"
           - Useful for computer security, bank transfers (like ATM
              cards), etc.
           - may have local intelligence (this is the usual sense)
           - microprocessors, observor protocol (Chaum)
           + Smart cards and electronic funds transfer
             - Tamper-resistant modules
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
  
  5.5. Cryptology-Technical, Mathematical
    5.5.1. Historical Cryptography
           + Enigma machines
             - cracked by English at Bletchley Park
             - a secret until mid-1970s
             + U.K. sold hundreds of seized E. machines to embassies,
                governments, even corporations, in late 1940s, early
                1950s
               - could then crack what was being said by allies
           + Hagelin, Boris (?)
             - U.S. paid him to install trapdoors, says Kahn
             + his company, Crypto A.G., was probably an NSA front
                company
               - Sweden, then U.S., then Sweden, then Zug
             - rotor systems cracked
    5.5.2. Public-key Systems--HISTORY
           + Inman has admitted that NSA had a P-K concept in 1966
             - fits with Dominik's point about sealed cryptosystem boxes
                with no way to load new keys
             - and consistent with NSA having essentially sole access to
                nation's top mathematicians (until Diffies and Hellmans
                foreswore government funding, as a result of the anti-
                Pentagon feelings of the 70s)
           - Merkle's "puzzle" ideas, circa mid-70s
           - Diffie and Hellman
           - Rivest, Shamir, and Adleman
    5.5.3. RSA and Alternatives to RSA
           + RSA and other P-K patents are strangling development and
              dissemination of crypto systems
             - perhaps out of marketing stupidity, perhaps with the help
                of the government (which has an interest in keeping a
                monopoly on secure encryption)
           + One-way functions and "deposit-only envelopes"
             - one-way functions
             - deposit-only envelopes: allow additions to envelopes and
                only addressee can open
           - hash functions are easy to implement one-way functions
              (with no need for an inverse)
    5.5.4. Digital Signatures
           + Uses of Digital Signatures
             - Electronic Contracts
             - Voting
             - Checks and other financial instruments (similar to
                contracts)
             - Date-stamped Transactions (augmenting Notary Publics)
           - Undeniable digital signatures
           + Unforgeable signatures, even with unlimited computational
              power, can be achieved if the population is limited (a
              finite set of agents)
             - using an untraceable sending protocol, such as "the
                Dining Cryptographers Problem" of Chaum
    5.5.5. Randomness and incompressibility
           + best definition we have is due to Chaitin and Kolmogoroff:
              a string or any structure is "random" if it has no shorter
              description of itself than itself.
             - (Now even specific instances of "randomly generated
                strings" sometimes will be compressible--but not very
                often. Cf. the works of Chaitin and others for more on
                these sorts of points.)
    5.5.6. Steganography: Methods for Hiding the Mere Existence of
            Encrypted Data
           + in contrast to the oft-cited point (made by crypto purists)
              that one must assume the opponent has full access to the
              cryptotext, some fragments of decrypted plaintext,  and to
              the algorithm itself, i.e., assume the worst
             - a condition I think is practically absurd and unrealistic
             - assumes infinite intercept power (same assumption of
                infinite computer power would make all systems besides
                one-time pads breakable)
             - in reality, hiding the existence and form of an encrypted
                message is important
             + this will be all the more so as legal challenges to
                crypto are mounted...the proposed ban on encrypted
                telecom (with $10K per day fine), various governmental
                regulations, etc.
               - RICO and other broad brush ploys may make people very
                  careful about revealing that they are even using
                  encryption (regardless of how secure the keys are)
           + steganography, the science of hiding the existence of
              encrypted information
             - secret inks
             - microdots
             - thwarting traffic analysis
             - LSB method
           + Packing data into audio tapes (LSB of DAT)
             + LSB of DAT: a 2GB audio DAT will allow more than 100
                megabytes in the LSBs
               - less if algorithms are used to shape the spectrum to
                  make it look even more like noise
               - but can also use the higher bits, too (since a real-
                  world recording will have noise reaching up to perhaps
                  the 3rd or 4th bit)
               + will manufacturers investigate "dithering"  circuits?
                  (a la fat zero?)
                 - but the race will still be on
           + Digital video will offer even more storage space (larger
              tapes)
             - DVI, etc.
             - HDTV by late 1990s
           + Messages can be put into GIFF, TIFF image files (or even
              noisy faxes)
             - using the LSB method, with a 1024 x 1024 grey scale image
                holding 64KB in the LSB plane alone
             - with error correction, noise shaping, etc., still at
                least 50KB
             - scenario: already being used to transmit message through
                international fax and image transmissions
           + The Old "Two Plaintexts" Ploy
             - one decoding produces "Having a nice time. Wish you were
                here."
             - other decoding, of the same raw bits, produces "The last
                submarine left this morning."
             - any legal order to produce the key generates the first
                message
             + authorities can never prove-save for torture or an
                informant-that another message exists
               - unless there are somehow signs that the encrypted
                  message is somehow "inefficiently encrypted, suggesting
                  the use of a dual plaintext pair method" (or somesuch
                  spookspeak)
             - again, certain purist argue that such issues (which are
                related to the old "How do you know when to stop?"
                question) are misleading, that one must assume the
                opponent has nearly complete access to everything except
                the actual key, that any scheme to combine multiple
                systems is no better than what is gotten as a result of
                the combination itself
           - and just the overall bandwidth of data...
           + Several programs exist:
             - Stego
             - etc. (described elsewhere)
    5.5.7. The Essential Impossibility of Breaking Modern Ciphers and
            Codes
           - this is an important change from the past (and from various
              thriller novels that have big computers cracking codes)
           - granted, "unbreakable" is a misleading term
           + recall the comment that NSA has not really broken any
              Soviet systems in many years
             - except for the cases, a la the Walker case, where
                plaintext versions are gotten, i.e., where human screwups
                occurred
           - the image in so many novels of massive computers breaking
              codes is absurd: modern ciphers will not be broken (but the
              primitive ciphers used by so many Third World nations and
              their embassies will continue to be child's play, even for
              high school science fair projects...could be a good idea
              for a small scene, about a BCC student who has his project
              pulled)
           + But could novel computational methods crack these public
              key ciphers?
             + some speculative candidates
               + holographic computers, where large numbers are
                  factored-or at least the possibilities are somehown
                  narrowed-by using arrays that (somehow) represent the
                  numbers to be factored
                 - perhaps with diffraction, channeling, etc.
               - neural networks and evolutionary systems (genetic
                  algorithms)
             - the idea is that somehow the massive computations can be
                converted into something that is inherently parallel
                (like a crystal)
             + hyperspeculatively: finding the oracle for these problems
                using nonconventional methods such as ESP and lucid
                dreaming
               - some groups feel this is worthwhile
    5.5.8. Anonymous Transfers
           - Chaum's digital mixes
           - "Dining Cryptographers"
           + can do it with exchanged diskettes, at a simple level
             - wherein each person can add new material
             + Alice to Bob to Carol....Alice and Carol can conspire to
                determine what Bob had added, but a sufficient "mixing"
                of bits and pieces is possible such that only if
                everybody conspires can one of the participants be caught
               - perhaps the card-shuffling results?
           + may become common inside compute systems...
             - by this vague idea I mean that various new OS protocols
                may call for various new mechanisms for exchanging
                information
    5.5.9. Miscellaneous Abstract Ideas
           - can first order logic predicates be proven in zero
              knowledge?
           - Riemannn hypothesis
           + P = NP?
             - would the universe change?
             - Smale has shown that if the squares have real numbers in
                them, as opposed to natural numbers (integers), then P =
                NP; perhaps this isn't surprising, as a real implies sort
                of a recursive descent, with each square having unlimited
                computer power
             + oracles
               - speculatively,  a character asks if Tarot cards, etc.,
                  could be used (in addition to the normal idea that such
                  devices help psychologically)
               - "a cascade of changes coming in from hundreds of
                  decimal places out"
           + Quantum cryptography
             - bits can be exchanged-albeit at fairly low
                efficiencies-over a channel
             - with detection of taps, via the change of polarizations
             + Stephen Wiesner wrote a 1970 paper, half a decade before
                the P-K work, which outlined this-not published until
                much later
               - speculate that the NSA knew about this and quashed the
                  publication
           + But could novel computational methods crack these public
              key ciphers?
             + some speculative candidates
               + holographic computers, where large numbers are
                  factored-or at least the possibilities are somehown
                  narrowed-by using arrays that (somehow) represent the
                  numbers to be factored
                 - perhaps with diffraction, channeling, etc.
               - neural networks and evolutionary systems (genetic
                  algorithms)
             - the idea is that somehow the massive computations can be
                converted into something that is inherently parallel
                (like a crystal)
             + hyperspeculatively: finding the oracle for these problems
                using nonconventional methods such as ESP and lucid
                dreaming
               - some groups feel this is worthwhile
           - links to knot theory
           - "cut and choose" protocols (= zero knowledge)
           + can a "digital coin" be made?
             - this is formally similar to the idea of an active agent
                that is unforgeable, in the sense that the agent or coin
                is "standalone"
             + bits can always be duplicated (unless tied to hardware,
                as with TRMs), so must look elsewhere
               + could tie the bits to a specific location, so that
                  duplication would be obvious or useless
                 - the idea is vaguely that an agent could be placed in
                    some location...duplications would be both detectable
                    and irrelevant (same bits, same behavior,
                    unmodifiable because of digital signature)
           + coding theory and cryptography at the "Discrete
              Mathematics"
             - http://www.win.tue.nl/win/math/dw/index.html
   5.5.10. Tamper-resistant modules (TRMs) (or tamper-responding)
           + usually "tamper-indicating", a la seals
             - very tough to stop tampering, but relatively easy to see
                if seal has been breached (and then not restored
                faithfully)
             - possession of the "seal" is controlled...this is the
                historical equivalent to the "private key" in a digital
                signature system, with the technological difficulty of
                forging the seal being the protection
           + usually for crypto. keys and crypto. processing
             - nuclear test monitoring
             - smart cards
             - ATMs
           + one or more sensors to detect intrusion
             - vibration (carborundum particles)
             - pressure changes (a la museum display cases)
             - electrical
             - stressed-glass (Corning, Sandia)
           + test ban treaty verification requires this
             - fiber optic lines sealing a missile...
             - scratch patterns...
             - decals....
           + Epoxy resins
             - a la Intel in 1970s (8086)
             + Lawrence Livermore: "Connoisseur Project"
               - gov't agencies using this to protect against reverse
                  engineering, acquisition of keys, etc.
             + can't stop a determined effort, though
               - etches, solvents, plasma ashing, etc.
               - but can cause cost to be very high (esp. if resin
                  formula is varied frequently, so that "recipe" can't be
                  logged)
             + can use clear epoxy with "sparkles" in the epoxy and
                careful 2-position photography used to record pattern
               - perhaps with a transparent lid?
           + fiber optic seal (bundle of fibers, cut)
             - bundle of fibers is looped around device, then sealed and
                cut so that about half the fibers are cut; the pattern of
                lit and
                unlit fibers is a signature, and is extremely difficult
                to reproduce
           - nanotechnology may be used (someday)
  
  5.6. Crypto Programs and Products
    5.6.1. PGP, of course
           - it's own section, needless to say
    5.6.2. "What about hardware chips for encryption?"
           - Speed can be gotten, for sure, but at the expense of
              limiting the market dramatically. Good for military uses,
              not so good for civilian uses (especially as most civilians
              don't have a need for high speeds, all other things being
              equal).
    5.6.3. Carl Ellison's "tran" and mixing various ciphers in chains
           - "tran.shar is available at ftp.std.com:/pub/cme
           -      des | tran | des | tran | des
           - to make the job of the attacker much harder, and to make
              differential cryptanalyis harder
           - "it's in response to Eli's paper that I advocated prngxor,
              as in:
                       des | prngxor | tran | des | tran | des
              with the DES instances in ECB mode (in acknowledgement of
              Eli's attack). The prngxor destroys any patterns from the
              input, which was the purpose of CBC, without using the
              feedback path which Eli exploited."[ Carl Ellison, 1994-07-
              15]
    5.6.4. The Blum-Blum-Shub RNG
           - about the strongest algorithmic RNG we know of, albeit slow
              (if they can predict the next bit of BBS, they can break
              RSA, so....
           - ripem.msu.edu:/pub/crypt/other/blum-blum-shub-strong-
              randgen.shar
    5.6.5. the Blowfish cipher
           + BLOWFISH.ZIP, written by Bruce Schneier,1994. subject of an
              article in Dr. Dobb's Journal:
             - ftp.dsi.unimi.it:/pub/security/crypt/code/schneier-
                blowfish.c.gz
  
  5.7. Related Ideas
    5.7.1. "What is "blinding"?"
           + This is a basic primitive operation of most digital cash
              systems. Any good textbook on crypto should explain it, and
              cover the math needed to unerstand it in detail. Several
              people have explained it (many times) on the list; here's a
              short explanation by Karl Barrus:
             - "Conceptually, when you blind a message, nobody else can
                read it.  A property about blinding is that under the
                right circumstances if another party digitally signs a
                blinded message, the unblinded message will contain a
                valid digital signature.
                
                "So if Alice blinds the message "I owe Alice $1000" so
                that it reads (say) "a;dfafq)(*&" or whatever, and Bob
                agrees to sign this message, later Alice can unblind the
                message Bob signed to retrieve the original.  And Bob's
                digital signature will appear on the original, although
                he didn't sign the original directly.
                
                "Mathematically, blinding a message means multiplying it
                by a number (think of the message as being a number).
                Unblinding is simply dividing the original blinding
                factor out." [Karl Barrus, 1993-08-24]
           + And another explanation by Hal Finney, which came up in the
              context of how to delink pharmacy prescriptions from
              personal identity (fears of medial dossiers(:
             - "Chaum's "blinded credential" system is intended to solve
                exactly this kind of problem, but it requires an
                extensive infrastructure.  There has to be an agency
                where you physically identify yourself.  It doesn't have
                to know anything about you other than some physical ID
                like fingerprints.  You and it cooperate to create
                pseudonyms of various classes, for example, a "go to the
                doctor" pseudonym, and a "go to the pharmacy" pseudonym.
                These pseudonyms have a certain mathematical relationship
                which allows you to re-blind credentials written to one
                pseudonym to apply to any other.  But the agency uses
                your physical ID to make sure you only get one pseudonym
                of each kind....So, when the doctor gives you a
                prescription, that is a credential applied to your "go to
                the doctor" pseudonym.  (You can of course also reveal
                your real name to the doctor if you want.)  Then you show
                it at the pharmacy using your "go to the pharmacy"
                pseudonym.  The credential can only be shown on this one
                pseudonym at the pharamacy, but it is unlinkable to the
                one you got at the doctor's.  " [Hal Finney, 1994-09-07]
    5.7.2. "Crypto protocols are often confusing. Is there a coherent
            theory of these things?"
           - Yes, crypto protocols are often expressed as scenarios, as
              word problems, as "Alice and Bob and Eve" sorts of
              complicated interaction protocols. Not exactly game theory,
              not exactly logic, and not exactly anything else in
              particular...its own area.
           - Expert systems, proof-of-correctness calculi, etc.
           - spoofing, eavesdropping, motivations, reputations, trust
              models
           + In my opinion, much more work is needed here.
             - Graphs, agents, objects, capabilities, goals, intentions,
                logic
             - evolutionary game theory, cooperation, defection, tit-for-
                tat, ecologies, economies
             - mostly ignored, to date, by crypto community
    5.7.3. The holder of a key *is* the person, basically
           - that's the bottom line
           - those that worry about this are free to adopt stronger,
              more elaborate systems (multi-part, passphrases, biometric
              security, limits on account access, etc.)
           - whoever has a house key is essentially able to gain access
              (not saying this is the legal situation, but the practical
              one)
    5.7.4. Strong crypto is helped by huge increases in processor power,
            networks
           + Encryption *always wins out* over cryptanalysis...gap grows
              greater with time
             - "the bits win"
           + Networks can hide more bits...gigabits flowing across
              borders, stego, etc.
             - faster networks mean more "degrees of freedom," more
                avenues to hide bits in, exponentially increasing efforts
                to eavesdrop and track
             - (However, these additional degrees of freedome can mean
                greater chances for slipping up and leaving clues that
                allow correlation. Complexity can be a problem.)
           + "pulling the plug" hurts too much...shuts down world
              economy to stop illegal bits ("naughty bits"?)
             - one of the main goals is to reach the "point of no
                return," beyond which pulling the plug hurts too much
             - this is not to say they won't still pull the plug, damage
                be damned
    5.7.5. "What is the "Diffie-Hellman" protocol and why is it
            important?"
           + What it is
             - Diffie-Hellman, first described in 1976, allows key
                exchange over insecure channels.
             + Steve Bellovin was one of several people to explaine D-H
                to the list (every few months someone does!). I'm
                including his explanation, despite its length, to help
                readers who are not cryptologists get some flavor of the
                type of math involved. The thing to notice is the use of
                *exponentiations* and *modular arithmetic* (the "clock
                arithmetic" of our "new math" childhoods, except with
                really, really big numbers!). The difficulty of inverting
                the exponention (the discrete log problem) is what makes
                this a cryptographically interesting approach.
               - "The basic idea is simple.  Pick a large number p
                  (probably a prime), and a base b that is a generator of
                  the group of integers modulo p. Now, it turns out that
                  given a known p, b, and (b^x) mod p, it's extremely
                  hard to find out x.  That's known as the discrete log
                  problem.
                  
                  "Here's how to use it.  Let two parties, X and Y, pick
                  random numbers x and y, 1 < x,y < p.  They each
                  calculate
                  
                      (b^x) mod p
                  
                  and
                  
                          (b^y) mod p
                  
                  and transmit them to each other.  Now, X knows x and
                  (b^y) mod p, so s/he can calculate (b^y)^x mod p =
                  (b^(xy)) mod p.  Y can do the same calculation.  Now
                  they both know (b^(xy)) mod p.  But eavesdroppers know
                  only (b^x) mod p and (b^y) mod p, and can't use those
                  quantities to recover the shared secret.  Typically, of
                  course, X and Y will use that shared secret as a key to
                  a conventional cryptosystem.
                  
                  "The biggest problem with the algorithm, as outlined
                  above, is that there is no authentication.  An attacker
                  can sit in the middle and speak that protocol to each
                  legitimate party.
                  
                  "One last point -- you can treat x as a secret key, and
                  publish
                  (b^X) mod p as a public key.  Proof is left as an
                  exercise for
                  the reader."  [Steve Bellovin, 1993-07-17]
           - Why it's important
           + Using it
             + Matt Ghio has made available Phil Karn's program for
                generating numbers useful for D-H:
               - ftp cs.cmu.edu:
                  /afs/andrew.cmu.edu/usr12/mg5n/public/Karn.DH.generator
           + Variants and Comments
             + Station to Station protocol
               - "The STS protocol is a regular D-H followed by a
                  (delicately designed) exchange of signatures on the key
                  exchange parameters.  The signatures in the second
                  exchange that they can't be separated from the original
                  parameters.....STS is a well-thought out protocol, with
                  many subtleties already arranged for.  For the issue at
                  hand, though, which is Ethernet sniffing, it's
                  authentication aspects are not required now, even
                  though they certainly will be in the near future."
                  [Eric Hughes, 1994-02-06]
    5.7.6. groups, multiple encryption, IDEA, DES, difficulties in
            analyzing
    5.7.7. "Why and how is "randomness" tested?"
           - Randomness is a core concept in cryptography. Ciphers often
              fail when things are not as random as designers thought
              they would be.
           - Entropy, randomness, predictablility. Can never actually
              _prove_ a data set is random, though one can be fairly
              confident (cf. Kolmogorov-Chaitin complexity theory).
           - Still, tricks can make a random-looking text block look
              regular....this is what decryption does; such files are
              said to be cryptoregular.
           + As to how much testing is needed, this depends on the use,
              and on the degree of confidence needed. It may take
              millions of test samples, or even more, to establish
              randomness in set of data. For example:
             - "The standard tests for 'randomness' utilized in govt
                systems requires 1X10^6 samples. Most of the tests are
                standard probability stuff and some are classified. "
                [Wray Kephart, sci.crypt, 1994-08-07]
             - never assume something is really random just becuase it
                _looks_ random! (Dynamic Markov compressors can find
                nonrandomness quickly.)
    5.7.8. "Is it possible to tell if a file is encrypted?"
           - Not in general. Undecideability and all that. (Can't tell
              in general if a virus exists in code, Adleman showed, and
              can't tell in general if a file is encrypted, compressed,
              etc. Goes to issues of what we mean by encrypted or
              compressed.)
           + Sometimes we can have some pretty clear signals:
             - headers are attached
             - other characteristic signs
             - entropy per character
           + But files encrypted with strong methods typically look
              random; in fact, randomness is closely related to
              encyption.
             + regularity: all symbols represented equally, in all bases
                (that is, in doubles, triples, and all n-tuples)
               - "cryptoregular" is the term: file looks random
                  (regular) until proper key is applied, then the
                  randomness vaDCharles Bennett, "Physics of Computation
                  Workshop," 1993]
             - "entropy" near the maximum (e.g., near 6 or 7 bits per
                character, whereas ordinary English has roughly 1.5-2
                bits per character of entropy)
    5.7.9. "Why not use CD-ROMs for one-time pads?"
           - The key distribution problem, and general headaches. Theft
              or compromise of the keying material is of course the
              greatest threat.
           - And one-time pads, being symmetric ciphers, give up the
              incredible advantages of public key methods.
           - "CD ROM is a terrible medium for the OTP key stream.
              First, you want exactly two copies of the random stream.
              CD ROM has an economic advantage only for large runs.
              Second, you want to destroy the part of the stream already
              used.  CD ROM has no erase facilities, outside of physical
              destruction of the entire disk." [Bryan G. Olson,
              sci.crypt, 1994-08-31]
           - If you have to have a one-time pad, a DAT makes more sense;
              cheap, can erase the bits already used, doesn't require
              pressing of a CD, etc. (One company claims to be selling CD-
              ROMs as one-time pads to customers...the security problems
              here should be obvious to all.)
  
  5.8. The Nature of Cryptology
    5.8.1. "What are the truly basic, core, primitive ideas of
            cryptology, crypto protocols, crypto anarchy, digital cash,
            and the things we deal with here?"
           - I don't just mean things like the mechanics of encryption,
              but more basic conceptual ideas.
    5.8.2. Crypto is about the creation and linking of private spaces...
    5.8.3. The "Core" Ideas of Cryptology and What we Deal With
           - Physics has mass, energy, force, momentum, angular
              momentum, gravitation, friction, the Uncertainty Principle,
              Complementarity, Least Action, and a hundred other such
              concepts and prinicples, some more basic than others. Ditto
              for any other field.
           + It seems to many of us that crypto is part of a larger
              study of core ideas involving: identity, proof, complexity,
              randomness, reputations, cut-and-choose protocols, zero
              knowledge, etc. In other words, the buzzwords.
             - But which of these are "core" concepts, from which others
                are derived?
             - Why, for example, do the "cut-and-choose" protocols work
                so well, so fairly? (That they do has been evident for a
                long time, and they literally are instances of Solomonic
                wisdom. Game theory has explanations in terms of payoff
                matrices, Nash equilibria, etc. It seems likely to me
                that the concepts of crypto will be recast in terms of a
                smaller set of basic ideas taken from these disparate
                fields of economics, game theory, formal systems, and
                ecology. Just my hunch.)
           + statements, assertions, belief, proof
             - "I am Tim"
             + possession of a key to a lock is usually treated as proof
                of...
               - not always, but that's the default assumption, that
                  someone who unlocks a door is one of the proper
                  people..access privileges, etc.
    5.8.4. We don't seem to know the "deep theory" about why certain
            protocols "work." For example, why is "cut-and-choose," where
            Alice cuts and Bob chooses (as in fairly dividing a pie),
            such a fair system? Game theory has a lot to do with it.
            Payoff matrices, etc.
           - But many protocols have not been fully studied. We know
              they work, but I think we don't know fully why they work.
              (Maybe I'm wrong here, but I've seen few papers looking at
              these issues in detail.)
           - Economics is certainly crucial, and tends to get overlooked
              in analysis of crypto protocols....the various "Crypto
              Conference Proceedings" papers typically ignore economic
              factors (except in the area of measuring the strength of a
              system in terms of computational cost to break).
           - "All crypto is economics."
           - We learn what works, and what doesn't. My hunch is that
              complex crypto systems will have emergent behaviors that
              are discovered only after deployment, or good simulation
              (hence my interest in "protocol ecologies").
    5.8.5. "Is it possible to create ciphers that are unbreakable in any
            amount of time with any amount of computer power?"
           + Information-theoretically secure vs. computationally-secure
             + not breakable even in principle, e.g., a one-time pad
                with random characters selected by a truly random process
                (die tosses, radioactive decay, certain types of noise,
                etc.)
               - and ignoring the "breakable by break-ins" approach of
                  stealing the one-time pad, etc. ("Black bag
                  cryptography")
             - not breakable in "reasonable" amounts of time with
                computers
           - Of course, a one-time pad (Vernam cipher) is theoretically
              unbreakable without the key. It is "information-
              theoretically secure."
           - RSA and similar public key algorithms are said to be only
              "computationally-secure," to some level of security
              dependent on modulus lenght, computer resources and time
              available, etc. Thus, given enough time and enough computer
              power, these ciphers are breakable.
           - However, they may be practically impossible to break, given
              the amount of energy in the universe.Not to split universes
              here, but it is interesting to consider that some ciphers
              may not be breakable in _our_ universe, in any amount of
              time. Our universe presumably has some finite number of
              particles (currently estimated to be 10^73 particles). This
              leads to the "even if every particle were a Cray Y-MP it
              would take..." sorts of thought experiments.
              
              But I am considering _energy_ here. Ignoring reversible
              computation for the moment, computations dissipate energy
              (some disagree with this point). There is some uppper limit
              on how many basic computations could ever be done with the
              amount of free energy in the universe. (A rough calculation
              could be done by calculating the energy output of stars,
              stuff falling into black holes, etc., and then assuming
              about kT per logical operation. This should be accurate to
              within a few orders of magnitude.) I haven't done this
              calculation, and won't today, but the result would likely
              be something along the lines of X joules of energy that
              could be harnessed for computation, resulting in Y basic
              primitive computational steps.
              
              I can then find a modulus of 3000 digits or 5000 digits, or
              whatever,that takes more than this number of steps to
              factor.
              
              Caveats:
              
              1. Maybe there are really shortcuts to factoring. Certainly
              improvements in factoring methods will continue. (But of
              course these improvements are not things that convert
              factoring into a less than exponential-in-length
              problem...that is, factoring appears to remain "hard.")
              
              2. Maybe reversible computations (a la Landauer, Bennett,
              et. al.) actually work. Maybe this means a "factoring
              machine" can be built which takes a fixed, or very slowly
              growing, amount of energy.
              
              3. Maybe the quantum-mechanical idea of Shore is possible.
              (I doubt it, for various reasons.)
              
              I continue to find it useful to think of very large numbers
              as creating "force fields" or "bobbles" (a la Vinge) around
              data. A 5000-decimal-digit modulus is as close to being
              unbreakable as anything we'll see in this universe.
  
  5.9. Practical Crypto
    5.9.1. again, this stuff is covered in many of the FAQs on PGP and
            on security that are floating around...
    5.9.2. "How long should crypto be valid for?"
           + That is, how long should a file remain uncrackable, or a
              digital signature remain unforgeable?
             - probabalistic, of course, with varying confidence levels
             - depends on breakthroughs, in math and in computer power
           + Some messages may only need to be valid for a few days or
              weeks. Others, for decades. Certain contracts may need to
              be unforgeable for many decades. And given advances in
              computer power, what appears to be a strong key today may
              fail utterly by 2020 or 2040.  (I'm of course not
              suggesting that a 300- or 500-digit RSA modulus will be
              practical by then.)
             + many people only need security for a matter of months or
                so, while others may need it (or think they need it) for
                decades or even for generations
               - they may fear retaliation against their heirs, for
                  example, if certain communications were ever made
                  public
           - "If you are signing the contract digitally, for instance,
              you would want to be sure that no one could forge your
              signature to change the terms after the fact -- a few
              months isn't enough for such purposes, only something that
              will last for fifteen or twenty years is okay." [Perry
              Metzger, 1994-07-06]
    5.9.3. "What about commercial encryption programs for protecting
            files?"
           - ViaCrypt, PGP 2.7
           - Various commercial programs have existed for years (I got
              "Sentinel" back in 1987-8...long since discontinued). Check
              reviews in the leading magazines.
           + Kent Marsh, FolderBolt for Macs and Windows
             - "The best Mac security program....is CryptoMactic by Kent
                Marsh Ltd.  It uses triple-DES in CBC mode, hashes an
                arbitrary-length password into a key, and has a whole lot
                of Mac-interface features.  (The Windows equivalent is
                FolderBolt for Windows, by the way.)" [Bruce Schneier,
                sci.crypt, 1994-07-19]
    5.9.4. "What are some practical steps to take to improve security?"
           - Do you, like most of us, leave backup diskettes laying
              around?
           - Do you use multiple-pass erasures of disks? If not, the
              bits may be recovered.
           - (Either of these can compromise all encrypted material you
              have, all with nothing more than a search warrant of your
              premises.)
    5.9.5. Picking (and remembering) passwords
           - Many of the issues here also apply to choosing remailers,
              etc. Things are often trickier than they seem. The
              "structure" of these spaces is tricky. For example, it may
              seem really sneaky (and "high entropy" to permute some
              words in a popular song and use that as a pass
              phrase....but this is obviously worth only a few bits of
              extra entropy. Specifically, the attacker will like take
              the thousand or so most popular songs, thousand or so most
              popular names, slogans, speeches, etc., and then run many
              permutations on each of them.
           - bits of entropy
           - lots of flaws, weaknesses, hidden factors
           - avoid simple words, etc.
           - hard to get 100 or more bits of real entropy
           - As Eli Brandt puts it, "Obscurity is no substitute for
              strong random numbers." [E.B., 1994-07-03]
           - Cryptanalysis is a matter of deduction, of forming and
              refining hypotheses. For example, the site
              "bitbucket@ee.und.ac.za" is advertised on the Net as a
              place to send "NSA food" to...mail sent to it gets
              discarded. So , a great place to send cover traffic to, no?
              No, as the NSA will mark this site for what it is and its
              usefulness is blown. (Unless its usefulness is actually
              something else, in which case the recursive descent has
              begun.)
           - Bohdan Tashchuk suggests [1994-07-04] using telephone-like
              numbers, mixed in with words, to better fit with human
              memorization habits; he notes that 30 or more bits of
              entropy are routinely memorized this way.
    5.9.6. "How can I remember long passwords or passphrases?"
           - Lots of security articles have tips on picking hard-to-
              guess (high entropy) passwords and passphrases.
           + Just do it.
             - People can learn to memorize long sequences. I'm not good
                at this, but others apparently are. Still, it seems
                dangerous, in terms of forgetting. (And writing down a
                passphrase may be vastly more risky than a shorter but
                more easily memorized passphrase is.  I think theft
                of keys and keystroke capturing on compromised machines
                are much
                more important practical weaknesses.)
           + The first letters of long phrases that have meaning only to
              the owner.
             - e.g., "When I was ten I ate the whole thing."--->
                "wiwtiatwt" (Purists will quibble that prepositional
                phrases like "when i was" have lower entropy. True, but
                better than "Joshua.")
           + Visual systems
             - Another approach to getting enough entropy in
                passwords/phrases is a "visual key" where one mouses from
                position to position in a visual environment. That is,
                one is presented with a scene containg some number of
                nodes, perhaps representing familiar objects from one's
                own home, and a path is chosen.  The advantage is that
                most people can remember fairly complicated
                (read: high entropy) "stories." Each object triggers a
                memory of the next object to visit. (Example: door to
                kitchen to blender to refrigerator to ..... ) This is the
                visual memory system said to be favored by Greek epic
                poets. This also gets around the keyboard-monitoring
                trick (but not necessarily the CRT-reading trick, of
                course).
                
                
                It might be an interesting hack to offer this as a front
                end for PGP. Even a simple grid of characters which could
                be moused on could be an assist in using long
                passphrases.
 
 5.10. DES
   5.10.1. on the design of DES
           - Biham and Shamir showed how "differential cryptanalyis"
              could make the attack easier than brute-force search of the
              2^56 keyspace. Wiener did a thought experiment design of a
              "DES buster" machine (who ya gonna call?) that could break
              a DES key in a matter of days. (Similar to the Diffie and
              Hellman analysis of the mid-70s, updated to current
              technology.)
           + The IBM designers knew about differential cryptanalyis, it
              is now clear, and took steps to optimize DES. After Shamir
              and Biham published, Don Coppersmith acknowledged this.
              He's written a review paper:
             - Coppersmith, D.,  "The Data Encryption Standard (DES) and
                its strength against attacks."  IBM Journal of Research
                and Development.  38(3): 243-250. (May 1994)
 
 5.11. Breaking Ciphers
   5.11.1. This is not a main Cypherpunks concern, for a variety of
            reasons (lots of work, special expertise, big machines, not a
            core area, ciphers always win in the long run). Breaking
            ciphers is something to consider, hence this brief section.
   5.11.2. "What are the possible consequences of weaknesses in crypto
            systems?"
           - maybe reading messages
           - maybe forging messages
           - maybe faking timestamped documents
           - maybe draining a bank account in seconds
           - maybe winning in a crypto gambling system
           - maybe matters of life and death
   5.11.3. "What are the weakest places in ciphers, practically
            speaking?"
           - Key management, without a doubt. People leave their keys
              lying around , write down their passphrases. etc.
   5.11.4. Birthday attacks
   5.11.5. For example, at Crypto '94 it was reported in a rump session
            (by Michael Wiener with Paul van Oorschot) that a machine to
            break the MD5 ciphers could be built for about $10 M (in 1994
            dollars, of course) and could break MD5 in about 20 days.
            (This follows the 1993 paper on a similar machine to break
            DES.)
           - Hal Finney did some calculations and reported to us:
           - "I mentioned a few days ago that one of the "rump session"
              papers at the crypto conference claimed that a machine
              could be built which would find MD5 collisions for $10M in
              about 20 days.....The net result is that we have taken
              virtually no more time (the 2^64 creations of MD5 will
              dominate) and virtually no space (compared to 2^64  stored
              values) and we get the effect of a birthday attack.  This
              is another cautionary data point about the risks of relying
              on space costs for security rather than time costs." [Hal
              Finney, 1994-09-09]
   5.11.6. pkzip reported broken
           - "I finally found time to take a closer look at the
              encryption algorithm by Roger Schlafly that is used in
              PKZIP and have developed a practical known plaintext attack
              that can find the entire 96-bit internal state." [Paul Carl
              Kocher, comp.risks, 1994-09-04]
   5.11.7. Gaming attacks, where loopholes in a system are exploited
           - contests that are defeated by automated attacks
           - the entire legal system can be viewed this way, with
              competing teams of lawyers looking for legal attacks  (and
              the more complex the legal code, the more attacks can be
              mounted)
           - ecologies, where weaknesses are exploited ruthlessly,
              forcing most species into extinction
           - economies, ditto, except must faster
           - the hazards for crypto schemes are clear
           + And there are important links to the issue of overly formal
              systems, or systems in which ordinary "discretion" and
              "choice" is overridden by rules from outside
             - as with rules telling employers in great detail when and
                how they can discharge employees (cf. the discussion of
                "reasonable rules made mandatory," elsewhere)
             - such rules get exploited by employees, who follow the
                "letter of the law" but are performing in a way
                unacceptable to the employer
             - related to "locality of reference" points, in that
                problem should be resolved locally, not with intervention
                from afar.
             - things will never be perfect, from the perspetive of all
                parties, but meddling from outside makes things into a
                game, the whole point of this section
           + Implications for digital money: overly complex legal
              systems, without the local advantages of true cash (settled
              locally)
             + may need to inject some supra-legal enforcement
                mechanisms into the system, to make it converge
               - offshore credit databases, beyond reach of U.S. and
                  other laws
               + physical violence (one reason people don't "play games"
                  with Mafia, Triads, etc., is that they know the
                  implications)
                 - it's not unethical, as I see it, for contracts  in
                    which the parties understand that a possible or even
                    likely consequence of their failure to perform is
                    death
   5.11.8. Diffie-Hellman key exchange vulnerabilities
           - "man-in-the-midle" attack
           + phone systems use voice readback of LCD indicated number
             - as computer power increases, even _this_ may be
                insufficient
   5.11.9. Reverse engineering of ciphers
           - A5 code used in GSM phones was reverse engineered from a
              hardware description
           - Graham Toal reports (1994-07-12) that GCHQ blocked a public
              lectures on this
 
 5.12. Loose Ends
   5.12.1. "Chess Grandmaster Problem" and other Frauds and Spoofs
           - of central importance to proofs of identity (a la Fiat-
              Shamir)
           - "terrorist" and "Mafia spoof" problems
