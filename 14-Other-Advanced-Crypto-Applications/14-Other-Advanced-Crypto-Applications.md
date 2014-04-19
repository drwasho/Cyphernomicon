14. Other Advanced Crypto Applications
 
 14.1. copyright
            THE  CYPHERNOMICON: Cypherpunks FAQ and More, Version 0.666,
            1994-09-10, Copyright Timothy C. May. All rights reserved.
            See the detailed disclaimer. Use short sections under "fair
            use" provisions, with appropriate credit, but don't put your
            name on my words.
 
 14.2. SUMMARY: Other Advanced Crypto Applications
   14.2.1. Main Points
   14.2.2. Connections to Other Sections
   14.2.3. Where to Find Additional Information
           - see the various "Crypto" Proceedings for various papers on
              topics that may come to be important
   14.2.4. Miscellaneous Comments
 
 14.3. Digital Timestamping
   14.3.1. digital timestamping
           - The canonical reference for digital timestamping is the
              work of Stu Haber and Scott Stornetta, of Bellcore. Papers
              presented at various Crypto conferences. Their work
              involves having the user compute a hash of the document he
              wishes to be stamped and sending the hash to them, where
              they merge this hash with other hashes (and all previous
              hashes, via a tree system) and then they *publish* the
              resultant hash in a very public and hard-to-alter forum,
              such as in an ad in the Sunday "New York Times."
              
              In their parlance, such an ad is a "widely witnessed
              event," and attempts to alter all or even many copies of
              the newspaper would be very difficult and expensive. (In a
              sense, this WWE is similar to the "beacon" term Eric Hughes
              used.)
              
              Haber and Stornetta plan some sort of commercial operation
              to do this.
              
              This service has not yet been tested in court, so far as I
              know. The MIT server is an experiment, and is probably
              useful for experimenting. But it is undoubtedly even less
              legally significant, of course.
   14.3.2. my summary
 
 14.4. Voting
   14.4.1. fraud, is-a-person, forging identies, increased "number"
            trends
   14.4.2. costs also high
   14.4.3. Chaum
   14.4.4. voting isomorphic to digital money
           - where account transfers are the thing being voted on, and
              the "eligible voters" are oneself...unless this sort of
              thing is outlawed, which would create other problems, then
              this makes a form of anonymous transfer possible (more or
              less)
 
 14.5. Timed-Release Crypto
   14.5.1. "Can anything like a "cryptographic time capsule" be built?"
           - This would be useful for sealing diaries and records in
              such a way that no legal bodies could gain access, that
              even the creator/encryptor would be unable to decrypt the
              records. Call it "time escrow." Ironically, a much more
              correct use of the term "escrow" than we saw with the
              government's various "key escrow" schemes.
           - Making records undecryptable is easy: just use a one-way
              function and the records are unreachable forever. The trick
              is to have a way to get them back at some future time.
           + Approaches:
             + Legal Repository. A lawyer or set of lawyers has the key
                or keys and is instructed to release them at some future
                time. (The key-holding agents need not be lawyers, of
                course, though that is the way things are now done.
               - The legal system is a time-honored way of protecting
                  secrets of various kinds, and any system based on
                  cryptography needs to compete strongly with this simple
                  to use, well-established system.
               - If the lawyer's identity is known, he can be
                  subpoenaed. Depends on jurisdictional issues, future
                  political climate, etc.
               - But identity-hiding protocols can be used, so that the
                  lawyer cannot be reached. All that is know, for
                  example, is that "somewhere out there" is an agent who
                  is holding the key(s). Reputation-based systems should
                  work well here: the agent gains little and loses a lot
                  by releasing a key early, hence has no economic
                  motivation to do so. (Picture also a lot of "pinging"
                  going to "rate" the various ti<w agents.)
             - Cryptography with Beacons. A "beacon agent" makes very
                public a series of messages, somehow. Details fuzzy. [I
                have a hunch that using digital time-stamping services
                could be useful here.]
             + Difficulty of factoring, etc.
               + The idea here is to-use a function which is presently
                  hard to invert, but which may be easier in the future.
                  This is fraught with problems, including
                  unpredictability of the difficulty, imprecision in the
                  timing of release, and general clumsiness. As Hal
                  Finney notes:
                 - "There was an talk on this topic at either the Crypto
                    92 or 93 conference, I forget which.  It is available
                    in the proceedings....The method used was similar to
                    the idea here of encrypting with a public key and
                    requiring factoring of the modulus to decrypt.  But
                    the author had more techniques he used, iterating
                    functions forward which would take longer to iterate
                    backwards.  The purpose was to give a more
                    predictable time to decrypt.....One problem with this
                    is that it does not so much put a time floor on the
                    decryption, but rather a cost floor.  Someone who is
                    willing to spend enough can decrypt faster than
                    someone who spends less.  Another problem is the
                    difficulty of forecasting the growth of computational
                    power per dollar in the future." [Hal Finney,
                    sci.crypt, 1994-8-04]
             + Tamper-resistant modules. A la the scheme to send the
                secrets to a satellite in orbit and expect that it will
                be prohibitively expensive to rendezvous and enter this
                satellite.
               - Or to gain access to tamper-resistant modules located
                  in bank vaults, etc.
               - But court orders and black bag jobs still are factors.
   14.5.2. Needs
           - journalism
           + time-stamping is a kind of example
             - though better seen in the conventional analysis
           - persistent institutions
           - shell games for moving money around, untraceably
   14.5.3. How
           - beacons
           - multi-part keys
           - contracted-for services (like publishing keys)
           - Wayner, my proposal, Eric Hughes
 
 14.6. Traffic Analysis
   14.6.1. digital form, and headers, LEAF fields, etc., make it vastly
            easier to know who has called whom, for how long, etc.
   14.6.2. (esp. in contrast to purely analog systems)
 
 14.7. Steganography
   14.7.1. (Another one of the topics that gets a lot of posts)
   14.7.2. Hiding messages in other messages
           - "Kevin Brown makes some interesting points about
              steganography and steganalysis.  The issue of recognizing
              whether a message has or mighthave a hidden message has two
              sides.  One is for the desired recipient to be clued that
              he should try desteganizing and decrypting the message, and
              the other is for a possible attacker to discover illegal
              uses of cryptography.
              
              "Steganography should be used with a "stealthy"
              cryptosystem (secret key or public key), one in which the
              cyphertext is indistinguishable from a random bit string.
              You would not want it to have any headers which could be
              used to confirm that a desteganized message was other than
              random noise." [Hal Finney, 1993-05-25]
   14.7.3. Peter Wayner's "Mimic"
           - "They encode a secret message inside a harmless looking
              ASCII text file.  This is one of the very few times
              the UNIX tools "lex" and "yacc" have been used in
              cryptography, as far as I know.   Peter Wayner, "Mimic
              Functions", CRYPTOLOGIA Volume 16, Number 3, pp. 193-214,
              July 1992.[Michael Johnson, sci.crypt, 1994-09-05]
   14.7.4. I described it in 1988 or 89 and many times since
           - Several years ago I posted to sci.crypt my "novel" idea for
              packing bits into the essentially inaudible "least
              significant bits" (LSBs) of digital recordings, such as
              DATs and CDs. Ditto for the LSBs in an 8-bit image or 24-
              bit color image. I've since seen this idea reinvented
              _several_ times on sci.crypt and elsewhere...and I'm
              willing to bet I wasn't the first, either (so I don't claim
              any credit).
              
              A 2-hour DAT contains about 10 Gbits (2 hours x 3600 sec/hr
              x 2 channels x 16 bits/sample x 44K samples/sec), or about
              1.2 Gbytes. A CD contains about half this, i.e., about 700
              Mbytes. The LSB of a DAT is 1/16th of the 1.2 Gbytes, or 80
              Mbytes. This is a _lot_ of storage!
              
              A home-recorded DAT--and I use a Sony D-3 DAT Walkman to
              make tapes--has so much noise down at the LSB level--noise
              from the A/D and D/A converters, noise from the microphones
              (if any), etc.--that the bits are essentially random at
              this level. (This is a subtle, but important, point: a
              factory recorded DAT or CD will have predetermined bits at
              all levels, i.e., the authorities could in principle spot
              any modifications. But home-recorded, or dubbed, DATs will
              of course not be subject to this kind of analysis.) Some
              care might be taken to ensure that the statistical
              properties of the signal bits resemble what would be
              expected with "noise" bits, but this will be a minor
              hurdle.
              
              Adobe Photoshop can be used to easily place message bits in
              the "noise" that dominates things down at the LSB level.
              The resulting GIF can then be posted to UseNet or e-mailed.
              Ditto for sound samples, using the ideas I just described
              (but typically requiring sound sampling boards, etc.). I've
              done some experiments along these lines.
              
              This doesn't mean our problems are solved, of course.
              Exchanging tapes is cumbersome and vulnerable to stings.
              But it does help to point out the utter futility of trying
              to stop the flow of bits.
   14.7.5. Stego, other versions
           - Romana Machado's Macintosh stego program is located in the
              compression files, /cmp, in the sumex-aim@stanford.edu info-
              mac archives.
           - "Stego is a tool that enables you to embed data in, and
              retrieve data from, Macintosh PICT format files, without
              changing the appearance of the PICT file.  Though its
              effect is visually undetectable, do not expect
              cryptographic security from Stego.  Be aware that anyone
              with a copy of Stego can retrieve your data from your PICT
              file.  Stego  can  be used as an "envelope" to hide a
              _previously encrypted_ data file in a PICT file, making it
              much less likely to be detected." [Romana Machado, 1993-11-
              23]
   14.7.6. WNSTORM, Arsen Ray Arachelian
   14.7.7. talk about it being used to "watermark" images
   14.7.8. Crypto and steganography used to plant false and misleading
            nuclear information
           - "Under a sub-sub-sub-contract I once worked on some phony
              CAD drawings for the nuclear weapons production process,
              plotting false info that still appears in popular books,
              some of which has been posted here....The docs were then
              encrypted and stegonagraphied for authenticity.  We were
              told that they were turned loose on the market for this
              product in other countries." [John Young, 1994-08-25]
           - Well...
   14.7.9. Postscript steganography
           - where info is embedded in spacings, font characteristics
              (angles, arcs)
           - ftp://research.att.com/dist/brassil/infocom94.ps
           - the essential point: just another haystack to hide a needle
 
 14.8. Hiding cyphertext
   14.8.1. "Ciphertext can be "uncompressed" to impose desired
            statistical properties.  A non-adaptive first-order
            arithmetic decompression will generate first-order symbol
            frequencies that emulate, for instance, English text." [Rick
            F. Hoselton, sci.crypt, 1994-07-05]
 
 14.9. 'What are tamper-responding or tamper-resistant modules?"
   14.9.1. The more modern name for what used to be called "tamper-proof
            boxes"
   14.9.2. Uses:
           - alarmed display cases, pressure-sensitive, etc. (jewels,
              art, etc.)
           + chips with extra layers, fuses, abrasive comounds in the
              packaging
             - to slow down grinding, etching, other depotting or
                decapping methods
             - VLSI Technology Inc. reportedly uses these methods in its
                implementation of the MYK-78 "Clipper" (EES) chip
           - nuclear weapons ("Permissive Action Links," a la Sandia,
              Simmons)
           - smartcards that give evidence of tampering, or that become
              inactive
           + as an example, disk drives that erase data when plug is
              pulled, unless proper code is first entered
             - whew! pretty risky (power failures and all), but needed
                by some
             - like "digital flash paper"
   14.9.3. Bypassing tamper-responding or tamper-resistant technologies
           - first, you have to _know_

14.10. Whistleblowing
  14.10.1. This was an early proposed use (my comments on it go back to
            1988 at least), and resulted in the creation of
            alt.whisteblowers.
           - So far, nothing too earth-shattering
  14.10.2. outing the secret agents of a country, by posting them
            anonymously to a world-wide Net distribution....that ought to
            shake things up

14.11. Digital Confessionals
  14.11.1. religious confessionals and consultations mediated by digital
            links...very hard for U.S. government to gain access
  14.11.2. ditto for attorney-client conversations, for sessions with
            psychiatrists and doctors, etc.
  14.11.3. (this does not meen these meetings are exempt from the
            law...witness Feds going after tainted legal fees, and
            bugging offices of attorneys suspected of being in the drug
            business)

14.12. Loose Ends
  14.12.1. Feigenbaum's "Computing with Encrypted Instances"
            work...links to Eric Hughes's "encrypted open books" ideas.
           - more work needed, clearly
