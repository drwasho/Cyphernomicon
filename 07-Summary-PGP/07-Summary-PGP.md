7.2. SUMMARY: PGP --  Pretty Good Privacy
    7.2.1. Main Points
           - PGP is the most important crypto tool there is, having
              single-handedly spread public key methods around the world
           - many other tools are being built on top of it
    7.2.2. Connections to Other Sections
           - ironically, almost no understanding of how PGP works in
              detail is needed; there are plenty of experts who
              specialize in that
    7.2.3. Where to Find Additional Information
           - newsgroups carry up to date comments; just read them for a
              few weeks and many things will float by
           - various FAQs on PGP
           + even an entire book, by Simpson Garfinkel:
             -   PGP: Pretty Good Privacy
                   by Simson Garfinkel
                   1st Edition November 1994 (est.)
                   250 pages (est),ISBN: 1-56592-098-8, $17.95 (est)
    7.2.4. Miscellaneous Comments
           - a vast number of ftp sites, URLs, etc., and these change
           - this document can't possibly stay current on these--see the
              pointers in the newsgroups for the most current sites
  
  7.3. Introduction
    7.3.1. Why does PGP rate its own section?
           - Like Clipper, PGP is too big a set of issues not to have
              its own section
    7.3.2. "What's the fascination in Cypherpunks with PGP?"
           - Ironically, our first meeting, in September 1992, coincided
              within a few days of the release of PGP 2.0. Arthur Abraham
              provided diskettes of 2.0, complete with laser-printed
              labels. Version 2.0 was the first truly useful version of
              PGP (so I hear....I never tried Version 1.0, which had
              limited distribution). So PGP and Cypherpunks shared a
              history--and Phil Zimmermann has been to some physical
              meetings.
           - A practical, usable, understandable tool. Fairly easy to
              use. In contrast, many other developments are more abstract
              and do not lend themselves to use by hobbyists and
              amateurs. This alone ensures PGP an honored place (and
              might be an object lesson for developers of other tools).
    7.3.3. The points here focus on PGP, but may apply as well to
            similar crypto programs, such as commercial RSA packages
            (integrated into mailers, commercial programs, etc.).
  
  7.4. What is PGP?
    7.4.1. "What is PGP?"
    7.4.2. "Why was PGP developed?"
    7.4.3. Who developed PGP?
  
  7.5. Importance of PGP
    7.5.1. PGP 2.0 arrived at an important time
           - in September 1992, the very same week the Cypherpunks had
              their first meeting, in Oakland, CA. (Arthur Abraham
              printed up professional-looking diskette labels for the PGO
              2.0 diskettes distributed. A general feeling that we were
              forming at the "right time.")
           - just 6 months before the Clipper announcement caused a
              firestorm of interest in public key cryptography
    7.5.2. PGP has been the catalyst for major shifts in opinion
           - has educated tens of thousands of users in the nature of
              strong crypto
           - has led to other tools, including encrypted remailers,
              experiments in digital money, etc.
    7.5.3. "If this stuff is so important, how come not everyone is
            digitally signing their messages?"
           - (Me, for example. I never sign my messages, and this FAQ is
              not signed. Maybe I will, later.)
           - convenience, ease of use, "all crypto is economics"
           - insecurity of host Unix machines (illusory)
           - better integration with mailers needed
    7.5.4. Ripem appears to be dead; traffic in alt.security.ripem is
            almost zero. PGP has obviously won the hearts and minds of
            the user community; and now that it's "legal"...
  
  7.6. PGP Versions
    7.6.1. PGP Versions and Implementations
           - 2.6ui is the version compatible with 2.3
           + What is the difference between versions 2.6 and 2.6ui?
             - "PGP 2.6 is distributed from MIT and is legally available
                to US and Canadian residents. It uses the RSAREF library.
                It has code that will prevent interoperation with earlier
                versions of PGP.
                "PGP 2.6ui is a modified version of PGP 2.3a which
                functions almost identically to MIT PGP 2.6, without the
                "cripple code" of MIT PGP 2.6. It is legally available
                outside the US and Canada only." [Rat
                <ratinox@ccs.neu.edu>, alt.security.pgp, 1994-07-03]
           + DOS
             - Versions
             + Pretty Good Shell
               - "When your Microsoft Mail supports an external Editor,
                  you might want to try PGS (Pretty Good Shell),
                  available as PGS099B.ZIP at several ftp sites. It
                  enables you to run PGP from a shell, with a easy way to
                  edit/encrypt files." [HHM LIMPENS, 1994-07-01]
           - Windows
           + Sun
             - "I guess that you should be able to use PGPsendmail,
                available at ftp.atnf.csiro.au:/pub/people/rgooch'
                [eric@terra.hacktic.nl (Eric Veldhuyzen), PGP support for
                Sun's Mailtool?, alt.security.pgp, 1994-06-29]
             + Mark Grant  <mark@unicorn.com> has been working on a tool
                to replace Sun's mailtool. "Privtool ("Privacy Tool") is
                intended to be a PGP-aware replacement for the standard
                Sun Workstation mailtool program, with a similar user
                interface and automagick support for PGP-signing and PGP-
                encryption." [MG, 1994-07-03]
               - "At the moment, the Beta release is available from
                  ftp.c2.org in /pub/privtool as privtool-0.80.tar.Z, and
                  I've attached the README.1ST file so that you can check
                  out the features and bugs before you download it. ....
                  Currently the program requires the Xview toolkit to
                  build, and has only been compiled on SunOS 4.1 and
                  Solaris 2.1."
           + MacPGP
             - 2.6ui: reports of problems, bombs (remove Preferencs set
                by previous versions from System folder)
             - "MacPGP 2.6ui is fully compatible with MIT's MacPGP 2.6,
                but offers several advantages, a chief one being that
                MacPGP 2.6ui is controllable via AppleScript.  This is a
                very powerful feature, and pre-written AppleScripts are
                already available.  A set of AppleScripts called the
                Interim Macintosh PGP Interface (IMPI) support
                encryption, decryption, and signing of files via drag-n-
                drop, finder selection, the clipboard, all accessible
                from a system-wide menu.  Eudora AppleScripts also exist
                to interface MacPGP with the mail program Eudora.
                
                "MacPGP 2.6ui v1.2 is available via anonymous ftp from:
                
                FTP SITE                 DIRECTORY
                CONTENTS
                --------                 ---------
                --------
                ftp.darmstadt.gmd.de     pub/crypto/macintosh/MacPGP
                MacPGP 2.6ui, source
                
                
                AppleScripts for 2.6ui are available for U.S. and
                Canadian citizens ONLY
                via anonymous ftp from:
                
                FTP SITE                 DIRECTORY
                CONTENTS
                --------                 ---------
                --------
                ftp.csn.net              mpj
                IMPI & Eudora scripts
                
                MacPGP 2.6ui, source
                [phinely@uhunix.uhcc.Hawaii.Edu (Peter Hinely),
                alt.security.pgp, 1994-06-28]
           - Amiga
           + VMS
             - 2.6ui is said to compile and run under VMS.
           + German version
             - MaaPGP0,1T1,1
             - dtp8//dtp,dapmqtadt,gmd,de/ilaomilg/MaaP
             - Ahpiqtoph_Pagalies@hh2.maus.
             - (source:  andreas.elbert@gmd.de (A.Elbert). by way of
                qwerty@netcom.com (-=Xenon=-), 3-31-94
    7.6.2. What versions of PGP exist?
           - PGP 2.7 is ViaCrypt's commercial version of PGP 2.6
    7.6.3. PGP 2.6 issues
           - There has been much confusion, in the press and in
              discussion groups, about the issues surrounding 2.5, 2.6,
              2.6ui, and various versions of these. Motivations,
              conspiracies, etc., have all been discussed. I'm not
              involved as others on our list are, so I'm often confused
              too.
           + Here are some comments by Phil Zimmermann, in response to a
              misleading press report:
             - "PGP 2.6 will always be able to read messages,
                signatures, and keys from olderversions, even after
                September 1st.  The older versions will not be able to
                read messages, signatures and keys produced by PGP 2.6
                after September 1st.  This is an entirely different
                situation.  There is every reason for people to switch to
                PGP 2.6, because it will be able to handle both data
                formats, while the older versions will not.  Until
                September, the new PGP will continue to produce the old
                format that can be read by older versions, but will start
                producing the new format after that date.  This delay
                allows time for everyone to obtain the new version of
                PGP, so that they will not be affected by the change.
                Key servers will still be able to carry the keys made in
                the old format, because PGP 2.6 will still read them with
                no problems. "  [Phil Zimmermann, 1994-07-07, also posted
                to Usenet groups] [all dates here refer to 1994]
             - "I developed PGP 2.6 to be released by MIT, and I think
                this new
                arrangement is a breakthrough in the legal status of PGP,
                of benefit to
                all PGP users.  I urge all PGP users to switch to PGP
                2.6, and abandon
                earlier versions.  The widespread replacement of the old
                versions with
                this new version of PGP fits in with future plans for the
                creation of a
                PGP standard."  [Phil Zimmermann, 1994-07-07, also posted
                to Usenet groups]
    7.6.4. PGP version 2.6.1
           - "MIT will be releasing Pretty Good Privacy (PGP) version
              2.6.1 real soon now.  By tomorrow, I think.  The MSDOS
              release filename will be pgp261.zip, and the source code
              will be in pgp261s.zip.  The MIT FTP site is net-
              dist@mit.edu, in the pub/PGP directory." [corrected by
              Derek Atkins to be: net-dist.mit.edu, not net-
              dist@mit.edu.]
              
              "This new version has a lot of bug fixes over version 2.6.
              I hope this is the final release of this family of PGP
              source code.  We've been working on an entirely new version
              of PGP, rewritten from scratch, which is much cleaner and
              faster, and better suited for the future enhancements we
              have planned.  All PGP development efforts will be
              redirected toward this new code base, after this 2.6.1
              release." [Phil Zimmermann, Cypherpunks list, 1994-09-02]
  
  7.7. Where to Get PGP?
    7.7.1. "Where can I get PGP on CompuServe?"
           - Note: I can't keep track of the major ftp sites for the
              various crypto packages, let alone info on services like
              this. But, here it is;
           - "Current as of 5-Jul-1994:"
              GO EURFORUM / Utilities   PGP26UI.ZIP   PGP 2.6ui
              GO PWOFORUM / New uploads PGP26.ZIP     PGP 2.6
               PWOFORUM also has the source code and documentation, plus
              a number of shell utilities for PGP.  Version 2.3a is also
              still around." [cannon@panix.com, Kevin Martin,  PGP on
              Compuserve??, alt.security.pgp, 1994-07-08]
    7.7.2. Off line PGP
           + ftp.informatik.uni-
              hamburg.de:/pub/virus/crypt/pgp/tools/pgp-elm.zip
             - another place: Crosspoint: ftp.uni-
                kl.de:/pub3/pc/dos/terminal/xpoint XP302*.EXE
           + "I highly recommend Offline AutoPGP v2.10.  It works
              seamlessly with virtually any offline mail reader that
              supports .QWK packets.  Shareware registration is $10.00
              US.  The author is Staale Schumacher, a student at the
              University of Oslo, is reachable at staale@ifi.uio.no .
              The program should be pretty widely available on US bbs's
              by now.  I use the program constantly for bbs mail.  It's
              really quite a slick piece of work.  If you have any
              trouble finding it, drop me a note."
              [bhowatt@eis.calstate.edu  Brent H. Howatt, PGP in an
              offline reader?, alt.security.pgp, 1994-07-05]
             - oak.oakland.edu in /pub/msdos/offline, version 2.11
             - ftp.informatik.uni-
                hamburg.de:/pub/virus/crypt/pgp/tools/apgp211.zip
    7.7.3. "Should I worry about obtaining and compiling the PGP
            sources?"
           - Well, unless you're an expert on the internals of PGP, why
              bother? And a subtle bug in the random number generator
              eluded even Colin Plumb for a while.
           - The value of the source being available is that others can,
              if they wish, make the confirmation that the executable
              correspond to the source. That this _can_ be done is enough
              for me. (Strategy: Hold on to the code for a while, wait
              for reports of flaws or holes, then use with confidence.)
           - Signatures can be checked. Maybe timestamped versions,
              someday.
           - Frankly, the odds are much higher that one's messages or
              pseudonymous identity will be exposed in others ways than
              that PGP has been compromised. Slip-ups in sending messages
              sometimes reveal identities, as do inadvertent comments and
              stylistic cues.
  
  7.8. How to Use PGP
    7.8.1. How does PGP work?
    7.8.2. "How should I store the secret part of my key? Can I memorize
            it?"
           - Modern ciphers use keys that are far beyond memorization
              (or even typing in!). The key is usually stored on one's
              home machine, or a machine that is reasonably secure, or on
              diskette. The passphrase should always be memorized or
              written down (ugh) in one's wallet or other such place.
              Secure "dongles" worn around the neck, or a ring or watch,
              may eventually be used. Smartcards and PDAs are a more
              likely intermediate solution (many PCs now have PCMCIA card
              slots).
    7.8.3. "How do I sign messages?"
           - cf. the PGP docs
           + however, this has come up on the List, and:
             -
             + pgp -sta +clearsig=on message.txt
               -
               - That's from pgpdoc2.txt.  Hope it helps.  You might
                  wish to set up your mail
               - user agent to invoke this command upon exiting your
                  default message editor,
               - with "message.txt" set to whatever your editor calls
                  the temporary message
               - file.               <Russell Whitaker,
                  whitaker@sgi.com, 4-15-94, Cypherpunks>
    7.8.4. Why isn't PGP easier to use?
           - Compared to other possible crypto applications (like
              digital money or voting systems), it is actually _very_
              easy to use
           - semantic gap...learning
    7.8.5. How should I learn PGP?
    7.8.6. "What's the status of PGP integration with other programs?"
           + Editors
             + emacs
               + emacs supports pgp, probably in various flavors (I've
                  seen several reports of different packages)..the built-
                  in language certainly helps
                 - Rick Busdiecker <rfb@lehman.com> has an emacs front
                    end to PGP available
                 - Jin S. Choi <jsc@monolith.MIT.EDU> once described a
                    package he wrote in elisp which supported GNU emacs:
                    "mailcrypt"
                 - there are probably many more
           + Mailers
             - That is, are there any mailers that have a good link to
                PGP? Hooks into existing mailers are needed
             + emacs
               + emacs supports pgp, probably in various flavors (I've
                  seen several reports of different packages)..the built-
                  in language certainly helps
                 - Rick Busdiecker <rfb@lehman.com> has an emacs front
                    end to PGP available
                 - Jin S. Choi <jsc@monolith.MIT.EDU> once described a
                    package he wrote in elisp which supported GNU emacs:
                    "mailcrypt"
                 - there are probably many more
             - elm
             - Eudora
             + PGP sendmail, etc.
               - "Get the PGPsendmail Suite, announced here a few days
                  ago. It's available for anonymous ftp from:
                  ftp.atnf.csiro.au: pub/people/rgooch   (Australia)
                  ftp.dhp.com: pub/crypto/pgp/PGPsendmail(U.S.A.)
                  ftp.ox.ac.uk: src/security  (U.K.)... It works by
                  wrapping around the regular  sendmail  programme, so
                  you get automatic encryption for all mailers, not just
                  Rmail. " [Richard Gooch, alt.security.pgp, 1994-07-10]
             + MIME
               - MIME and PGP <Derek Atkins, 4-6-94>
               - [the following material taken from an announcement
                  forwarded to the Cypherpunks list by
                  remijn@athena.research.ptt.nl, 1994-07-05]
               - "MIME [RFC-1341,  RFC-1521] defines a format and
                  general framework for the representation of a wide
                  variety of data types in Internet mail.  This document
                  defines one particular type of MIME data, the
                  application/pgp type, for "pretty good" privacy,
                  authentication, and encryption in Internet mail.  The
                  application/pgp MIME type is intended to facilitate the
                  wider  interoperation of private mail across a wide
                  variety of hardware and software platforms.
           + Newsreaders
             - useful for automatic signing/verification, and e-mail
                from withing newsreader
             - yarn
             - tin
             - The "yarn" newsreader reportedly has PGP built in.
    7.8.7. "How often should I change my key or keys?"
           - Hal Finney points out that many people seem to think PGP
              keys are quasi-permanent. In fact, never changing one's key
              is an invitation to disaster, as keys may be compromised in
              various ways (keystroke capture programs, diskettes left
              lying around, even rf monitoring) and may conceivably be
              cracked.
           - "
           + "What is a good interval for key changes?  I would suggest
              every year or so
             - makes sense, especially if infrastructure can be
                developed to make it easier
             - to propagate key changes.  Keys should be overlapped in
                time, so that you make
             - a new key and start using it, while continuing to support
                the old key for a
             - time. <Hal Finney, hfinney@shell.portal.com, 4-15-94,
                cypherpunks>
           - Hal also recommends that remailer sites change their keys
              even more frequently, perhaps monthly.
  
  7.9. Keys, Key Signings, and Key Servers
    7.9.1. Web of trust vs. heierarchical key management
           - A key innovations of Phil Zimmermann was the use of a "web
              of trust" model for distributed trust in keys.
           - locality, users bear costs
           - by contrast, government estimates $1-2 B a year to run key
              certification agencies for a large fraction of the
              population
           - "PGP is about choice and constructing a web of trust that
              suits your needs. PGP supports a completely decentralized,
              personalized web of trust and also the most highly
              structured bureaucratic centralized scheme you could
              imagine. One problem with relying solely on a personalized
              web of trust is that it limitsyour universe of
              correspondents. We can't expect Phil Zimmermann and a few
              well-known others to sign everyone's key, and I would not
              want to limit my private correspondence to just those
              people I know and trust plus those people whose keys have
              been signed by someone I know and trust." [William
              Stallings, SLED key verification, alt.security.pgp, 1994-09-
              01]
    7.9.2. Practical approaches to signing the keys of others
           + sign keys of folks you know and wish to communicate with
             - face-to-face encounters ("Here  is my key.")
           + trust--to varying extents--the keys signed by others you
              know
             - web-of-trust
           - trust--to a lesser extent--the keys of people in key
              registries
    7.9.3. Key Servers
           + There are several major sites which appear to be stable
             + MIT PGP Public Key Server
               - via www.eff.org
             + Vesselin Bontchev at University of Hamburg operates a
                very stable one:
               - Ftp:    ftp.informatik.uni-hamburg.de
                  IP:     134.100.4.42
                  Dir:    /pub/virus/crypt/pgp/
                  File:   pubkring.pgp
                  E-Mail: pgp-public-keys@fbihh.informatik.uni-hamburg.de
             - pgpkeys.io.com
           + http://martigny.ai.mit.edu/~bal/pks-commands.html
             - This is a PGP keyserver in Zurich.   <Russell Whitaker, 7
                April 1994>
             -
    7.9.4. Use of PGP key fingerprints
           - "One of the better uses for key fingerprints is for
              inclusion in signature files and other places that a key
              itself is too bulky.  By widespread dissemination of the
              fingerprint, the chances of a bogus key being undetected
              are decreased, since there are more channels for the
              fingerprint to get to recipients, and more channels for the
              owner of a key to see any bogus fingerprints out on the
              net. [Bill Stewart, 1994-08-31]
    7.9.5. "How should address changes be handled? Do old keys have to
            be revoked?"
           - Future versions of PGP may handle better
           - One way is to issue .... "User-id revocation certificates
              are a *good* idea and the PGP key format allows for them -
              maybe one day PGP will do something about it." [Paul Allen,
              alt.security.pgp, 1994-07-01]
           - Persistent e-mail addresses is one approach. Some  people
              are using organization like the ACM to provide this (e.g.,
              Phil Zimmermann is prz@acm.org). Others are using remapping
              services.  For example, "I signed up with the SLED (Stable
              Large E-mail Database), which is a cross-referencing
              database for linking old, obsolete E-mail addresses with
              current ones over the course of time.... Anyone using this
              key will always be able to find me on the SLED by
              conducting a search with "blbrooks..." as the keyword. Thus
              my key and associated sigs always remain good....  If you
              are interested in the SLED, its address is
              sled@drebes.com." [Robert Brooks, alt.security.pgp, 1994-07-
              01]
    7.9.6. "How can I ensure that my keys have not been tampered with?"
           + Keep your private key secure
             + if on an unsecured machine, take steps to protect it
               - offlline storage (Perry Metzger loads his key(s) every
                  morning, and removes it when he leaves the machine)
             + memorize your PGP passphrase and don't write it down, at
                least not anywhere near where the private key is
                available
               - sealed envelopes with a lawyer, safe deposit boxes,
                  etc., are possibilities
               - given the near-impossibility of recovering one's files
                  if the passphrase is lost permanently, I recommend
                  storing it _someplace_, despite the slight loss in
                  security (this is a topic of debate...I personally feel
                  a lot more comfortable knowing my memory is backed up
                  somewhere)
           - Colin Plumb has noted that if someone has accesss to your
              personal keyring, they also probably have access to your
              PGP program and could make modifications to it *directly*.
           - Derek Atkins answered a similar question on sci.crypt:
              "Sure.  You can use PGP to verify your keyring, and using
              the web-of-trust, you can then have it verify your
              signatures all the keys that you signed, and recurse
              through your circle-of-friends.  To verify that your own
              key was not munged, you can sign something with your secret
              key and then try to verify it.  This will ensure that your
              public key wasn't munged." [Derek Atkins, sci.crypt, 1994-
              07-06]
    7.9.7. "Why are key revocations needed?"
           - Key revocation is the "ebb-of-trust"
           - "There are a number of real reasons.  Maybe you got coerced
              into signing the key, or you think that maybe the key was
              signed incorrectly, or maybe that person no longer uses
              that email address, because they lost the account, or that
              maybe you don't believe that the binding of key to userID
              is valid for any number of reasons." [Derek Atkins, 4-28-
              94]
    7.9.8. "Is-a-person" registries
           + There have been proposals that governments could and should
              create registries of "legal persons." This is known in the
              crypto community as "is-a-person" credentialling, and
              various papers (notably Fiat-Shamir) have dealt with issues
             - of spoofing by malicious governments
             - of the dangers of person-tracking
           + We need to be very careful here!
             - this could limit the spread of 'ad hoc crypto' (by which
                I mean the use of locally-generated keys for reasons
                other than personal use...digital cash, pseudonyms etc.)
             - any system which "issues" permission slips to allow keys
                to be generated is dangerous!
           + Could be an area that governments want to get into.
             - a la Fiat-Shamir "passport" issues (Murdoch, Libyan
                example)
           - I favor free markets--no limitations on which registries I
              can use
    7.9.9. Keyservers (this list is constantly changing, but most share
            keys, so all one needs is one). Send "help" message. For
            current information, follow alt.security.pgp.
           - about 6000 keys on the main keyservers, as of 1994-08.
           - pgp-public-keys@martigny.ai.mit.edu
           - pgp-public-keys@dsi.unimi.it
           - pgp-public-keys@kub.nl
           - pgp-public-keys@sw.oz.au
           - pgp-public-keys@kiae.su
           - pgp-public-keys@fbihh.informatick.uni-hamburg.de
           - and wasabi.io.com offers public keys by finger (I couldn't
              get it to work)
   7.9.10. "What are key fingerprints and why are they used?"
           - "Distributing the key fingerprint allows J. Random Human to
              correlate a key supplied via one method with that supplied
              via another. For example, now that I have the fingerprint
              for the Betsi key, I can verify whether any other alleged
              Betsi key I see is real or not.....It's a lot easier to
              read off & cross-check 32-character fingerprints than the
              entire key block, especially as signatures are added and
              the key block grows in size." [Paul Robichaux, 1994-08-29]
   7.9.11. Betsi
           - Bellcore
           - key signing
   7.9.12. on attacks on keyservers...
           + flooding attacks on the keyservers have started; this may
              be an attempt to have the keyservers shut down by using
              obscene, racist, sexist phrases as key names (Cypherpunks
              would not support shutting down a site for something so
              trivial as abusive, offensive language, but many others
              would.)
             - "It appears that some childish jerk has had a great time
                generating bogus PGP keys and uploading them to the
                public keyservers. Here are some of the keys I found on a
                keyserver:...[keys elided]..." [staalesc@ifi.uio.no,
                alt.security.pgp, 1994-09-05]
 
 7.10. PGP Front Ends, Shells, and Tools
   7.10.1. Many can be found at this ftp site:
           + ftp.informatik.uni-hamburg.de:/pub/virus/crypt/pgp/shells/
             - for various shells and front-ends for PGP
   7.10.2. William Stallings had this to say in a Usenet post:
           - "PGPShell: runs directly on the DOS version, doesn't need
              Windows. Nice, simple interface. freeware
              
              "PGP Winfront: freeware windows front end. Uses a "control
              panel" style, with many options displayed in a compact
              fashion.
              
              "WinPGP: shareware ($45). Uses a drop-down menu style,
              common to many Windows applications." [William Stallings,
              Looking for PGP front end, alt.security, 1994-08-31]
   7.10.3. Rick Busdiecker <rfb@lehman.com> has an emacs front end to
            PGP available
   7.10.4. Pr0duct Cypher's tools:
           + ftp.informatik.uni-
              hamburg.de:/pub/virus/crypt/pgp/tools/PGPTools.tar.gz
             - Pr0duct Cypher's tools, and other tools in general
 
 7.11. Other Crypto Programs And Tools
   7.11.1. Other Ciphers and Tools
           - RIPEM
           - PEM
           - MD5
           + SFS (Secure FileSystem) 1.0
             - "SFS (Secure FileSystem) is a set of programs which
                create and manage a number of encrypted disk volumes, and
                runs under both DOS and Windows.  Each volume appears as
                a normal DOS drive, but all data stored on it is encryped
                at the individual-sector level....SFS 1.1 is a
                maintenance release which fixes a few minor problems in
                1.0, and adds a number of features suggested by users.
                More details on changes are given in in the README file."
                [Peter Gutmann, sci.crypt, 1994-08-25]
             - not the same thing as CFS!
             - 512-bit key using a MDC/SHS hash. (Fast)
             - only works on a386 or better (says V. Bontchev)
             - source code not available?
             - implemented as a device driver (rather than a TSR, like
                SecureDrive)
             - "is vulnerable to a special form of attack, which was
                mentioned once here in sci.crypt and is described in
                detaills in the SFS documentation. Take a loot at the
                section "Encryption Considerations"." [Vesselin Bontchev,
                sci.crypt, 1994-07-01]
             - Comparing SFS to SecureDrive: "Both packages are
                approximately equal in terms of user interface, but SFS
                seems to be quite a bit faster.  And comments from
                various people (previous message thread) seems to
                indicate that it is more "secure" as well." [Bill Couture
                <coutu001@gold.tc.umn.edu> , sci.crypt, 1994-0703]
           + SecureDrive
             - encrypts a disk (always be very careful!)
             - SecureDrive 1.3D, 128-bit IDEA cypher is based on an MD5
                hash of the passphrase
             - implemented as a TSR (rather than a device driver, like
                CFS)
             - source code available
             + Some problems reported (your mileage may vary)
               - "I have been having quite a bit of difficulty with my
                  encrypted drive mangling files. After getting secure
                  drive 1.3d installed on my hard drive, I find that
                  various files are being corrupted and many times after
                  accessing the drive a bunch of crosslinked files are
                  present." [Vaccinia@uncvx1.oit.unc.edu, 1994-07-01]
             - Others report being happy with, under both DOS and
                Windows
             - no OS/2 or Mac versions reported; some say an OS/2 device
                driver will have to be used (such as Stacker for OS/2
                uses)
           + SecureDevice
             - "If you can't find it elsewhere, I have it at
                ftp://ftp.ee.und.ac.za/pub/crypto/secdev13.arj, but
                that's at the end of a saturated 64kbps link." [Alan
                Barrett, 1994-07-01]
   7.11.2. MDC and SHS (same as SHA?)
           - "The MDC cyphers are believed to be as strong as it is
              difficult to invert the cryptographic hash function they
              are using. SHS was designed by the NSA and is believed to
              be secure. There might be other ways to attack the MDC
              cyphers, but nobody who is allowed to speak knows such
              methods."  [Vesselin Bontchev, sci.crypt, 1994-07-01]
           + Secure Hash Standard's algorithm is public, and hence can
              be analyzed and tested for weaknesses (in strong contrast
              with Skipjack).
             - may replace MD5 in future versions of PGP (a rumor)
           - Speed of MDC: "It's a speed tradeoff.  MDC is a few times
              faster than IDEA, so SFS is a few times faster than
              SecureDrive.  But MDC is less proven." [Colin Plumb,
              sci.crypt, 1994-07-04]
           + Rumors of problems with SHA
             - "The other big news is a security problem with the Secure
                Hash Algorithm (SHA), discussed in the Apr 94 DDJ.  The
                cryptographers at NSA have found a problem with the
                algorithm.  They won't tell anyone what it is, or even
                how serious it is, but they promise a fix soon.  Everyone
                is waiting with baited breath." [Bruce Schneier, reprot
                on Eurocrypt '94, 1994-07-01]
   7.11.3. Stego programs
           + DOS
             - S-Tools (or Stools?). DOS? Encrypts in .gif and .wav
                (SoundBlaster format) files. Can set to not indicate
                encrypted files are inside.
           - Windows
           + Macintosh
             - Stego
             + sound programs
               - marielsn@Hawaii.Edu (Nathan Mariels) has written a
                  program which "takes a file and encrypts it with IDEA
                  using a MD5 hash of the password typed in by the user.
                  It then stores the file in the lowest bit (or bits,
                  user selectable) of a sound file."
   7.11.4. "What about "Pretty Good Voice Privacy" or "Voice PGP" and
            Other Speech Programs?"
           + Several groups, including one led by Phil Zimmermann, are
              said to be working on something like this. Most are using
              commercially- and widely-available sound input boards, a la
              "SoundBlaster" boards.
             - proprietary hardware or DSPs is often a lose, as people
                won't be able to easily acquire the hardware; a software-
                only solution (possibly relying on built-in hardware, or
                readily-available add-in boards, like SoundBlasters) is
                preferable.
           + Many important reasons to do such a project:
             - proliferate more crypto tools and systems
             - get it out ahead of "Digital Telephony II" and Clipper-
                type systems; make the tools so ubiquitous that outlawing
                them is too difficult
             - people understand voice communcations in a more natural
                way than e-,mail, so people who don't use PGP may
                nevertheless use a voice encryption system
           + Eric Blossom has his own effort, and has demonstrated
              hardware at Cypherpunks meetings:
             - "At this moment our primary efforts are on developing a
                family of extensible protocols for both encryption and
                voice across point to point links.  We indend to use
                existing standards where ever possible.
                
                "We are currently planning on building on top of the RFCs
                for PPP (see RFCs 1549, 1548, and 1334).  The basic idea
                is to add a new Link Control Protocol (or possibly a
                Network Control Protocol) that will negotiate base and
                modulus and perform DH key exchange.  Some forms of
                Authentication are already supported by RFCs.  We're
                looking at others." [Eric Blossom, 1994-04-14]
           + Building on top of multimedia capabilities of Macintoshes
              and Windows may be an easier approach
             - nearly all Macs and Windows machines will be
                multimedia/audiovisual-capable soon
             - "I realize that it is quite possible to design a secure
                phone
                with a Vocoder, a modem and some cpu power to do the
                encryption, but I think that an easier solution may be on
                the horizon. ....I believe that Microsoft and many others
                are exploring hooking phones to PCs so people can do
                things like ship pictures of their weekend fun to
                friends. When PC's can easily access phone
                communications, then developing encrypted conversations
                should be as easy as programming for Windows :-)."
                [Peter Wayner, 1993--07-08]
   7.11.5. Random Number Generators
           - A huge area...
           + Chaotic systems, pendula
             - may be unexpected periodicities (phase space maps show
                basins of attraction, even though behavior is seemingly
                random)
   7.11.6. "What's the situation on the dispute between NIST and RSADSI
            over the DSS?"
           - NIST claims it doesn't infringe patents
           - RSADSI bought the Schnorr patent and claims DSS infringes
              it
           - NIST makes no guarantees, nor does it indemnify users
              [Reginald Braithwaite-Lee, talk.politics.crypto, 1994-07-
              04]
   7.11.7. "Are there any programs like telnet or "talk" that use pgp?"
           - "Don't know about Telnet, but I'd like to see "talk"
              secured like that...  It exists. (PGP-ized ytalk, that is.)
              Have a look at ftp.informatik.uni-
              hamburg.de:/pub/virus/crypto/pgp/tools/pgptalk.2.0.tar.gz"
              [Vesselin Bontchev, alt.security.pgp, 1994-07-4]
   7.11.8. Digital Timestamping
           + There are two flavors:
             - toy or play versions
             - real or comercial version(s)
           + For a play version, send a message to
              "timestamp@lorax.mv.com" and it will be timestamped and
              returned. Clearly this is not proof of much, has not been
              tested in court, and relies solely on the reputation of the
              timestamper. (A fatal flaw: is trivial to reset system
              clocks on computes and thereby alter dates.)
             - "hearsay" equivalent: time stamps by servers that are
                *not* using the "widely witnessed event" approach of
                Haber and Stornetta
           - The version of Haber and Stornetta is of course much more
              impressive, as it relies on something more powerful than
              mere trust that they have set the system clocks on their
              computers correctly!
 
 7.12. Legal Issues with PGP
   7.12.1. "What is RSA Data Security Inc.'s position on PGP?"
          I. They were strongly opposed to early versions
         II. objections
             - infringes on PKP patents (claimed infringements, not
                tested in court, though)
             - breaks the tight control previously seen
             - brings unwanted attention to public key approaches (I
                think PGP also helped RSA and RSADSI)
             - bad blood between Zimmermann and Bidzos
        III. objections
             - infringes on PKP patents (claimed infringements, not
                tested in court, though)
             - breaks the tight control previously seen
             - brings unwanted attention to public key approaches (I
                think PGP also helped RSA and RSADSI)
             - bad blood between Zimmermann and Bidzos
         IV. Talk of lawsuits, actions, etc.
          V. The 2.6 MIT accomodation may have lessened the tension;
              purely speculative
   7.12.2. "Is PGP legal or illegal"?
   7.12.3. "Is there still a conflict between RSADSI and PRZ?"
           - Apparently not. The MIT 2.6 negotiations seem to have
              buried all such rancor. At least officially. I hear there's
              still animosity, but it's no longer at the surface. (And
              RSADSI is now facing lawsuits and patent suits.)
 
 7.13. Problems with PGP, Flaws, Etc.
   7.13.1. Speculations on possible attacks on PGP
           + There are periodically reports of problems, most just
              rumors. These are swatted-down by more knowledgeable
              people, for the most part. True flaws may exist, of course,
              as in any piece of software.
             - Colin Plumb acknowledged a flaw in the random number
                generation process in PGP 2.6, to be fixed in later
                versions.
           + spreading fear, uncertainty and doubt
             - rumors about security of PGP versions
             - selective prosecution of PGP users
             - death threats (a la against Bidzos)
           - sowing confusion in the user community
           - fragmenting it (perhaps via multiple, noninteroperable
              versions...such as we're beginning to see now?)
   7.13.2. What does the NSA know about flaws in PGP?
           - They're not saying. Ironically, this violates the part of
              their charter that deals with making commercial security
              stronger. Now that PGP is kosher, they should help to make
              it stronger, and certainly should not keep mum about
              weaknesses they know about. But for them to help strengthen
              PGP is not really too likely.
   7.13.3. The PGP timebomb
           - (As I've said elsewhere, it all gets very confusing. Many
              versions, many sites, many viewpoints, many tools, many
              shells, many other things. Fortunately, most of it is
              flotsam.)
           - I take no point of view--for various reasons--on avoiding
              the "timebomb" by using 2.6ui. Here's someone else's
              comment:  "I would like to take this time to encourage you
              to upgrade to 2.6ui which will overcome mit's timebomb and
              not exclude PGP 2.3a from decrypting messages.....DON'T USE
              MIT's 2.6, use PGP 2.6ui available from soda.berkeley.edu
              : /pub/cypherpunks/pgp" [Matrix at Cypherpunks, BLACK
              THURSAY!, alt.security.pgp, 1994-09-01]
           + can also be defeated with the "legal kludge":
             - ftp.informatik.uni-hamburg.de :
                /pub/virus/crypt/pgp/legal_kludge.txt
   7.13.4. Spoofing
           - "Suitable timing constraints, and in particular real-time
              constraints, can be used to hinder, and perhaps defeat,
              spoofing attacks.  But with a store-and-forward e-mail
              system (such as PGP is designed to work with) these
              constraints cannot, in general, be set." [Ken Pizzini ,
              sci.crypt, 1994-07-05]
   7.13.5. "How do we know that PGP doesn't have a back door or some
            other major flaw? After all, not all of us are programmers or
            cryptologists."
           - Yes, but many of us are. Many folks have analyzed the
              source code in PGP, have compiled the code themselves (a
              fairly common way to get the executable), and have examined
              the random number generators, the selection of primes, and
              all of the other math.
           + It would take only a single sharp-eyed person to blow the
              whistle on a conspiracy to insert flaws or backdoors. This
              has not been done. (Though Colin Plumb ackknowledged a
              slight weakness in the RNG of 2.6...being fixed.)
             - "While having source code available doesn't guarantee
                that the program is secure, it helps a lot.  Even though
                many users are not programmers or cryptographers, others
                are, and many of these will examine the code    carefully
                and publicly yell about weaknesses that they notice or
                think they notice.  For example, apparently there was a
                big discussion here about the xorbytes() bug in PGP 2.6.
                Contrast this with a commercial program, where such a bug
                might go undetected for years." [Paul Rubin,
                alt.security.pgp, 1994-09-06]
   7.13.6. "Can I run PGP on a machine I don't control, e.g., the campus
            computer system?"
           - Sure, but the sysops and others may then have access to
              your key and passphrase. Only machines the user directly
              controls, and that are adequately firewalled from other
              machines, offer reasonable amounts of security.  Arguing
              about whether 1024-bit keylengths are "enough" is rather
              moot if the PGP program is being run on a corportate
              computer, or a university network. The illusion of security
              may be present, but no real security. Too many people are
              kidding themselves that their messages are secure.  That
              their electronic identities cannot be spoofed.
           - I'm not interested in the various elm and emacs PGP
              packages (several such shells and wrappers exist). Any
              sysop can not only obtain your secret key, stored on
              hissystem, but he can also capture your passphrase as you
              feed it to the PGP program (assuming you do...many people
              automate this part as well). Since this sysop or one of his
              cronies can then compromise your mail, sign messages and
              contracts as "you," I consider this totally unacceptable.
              Others apparently don't.
           - What can be done? Many of us only run PGP on home machines,
              or on machines we directly control. Some folks who use PGP
              on such machines at least take steps to better secure
              things....Perry Metzger, for example, once described the
              multi-stage process he went through each day to reload his
              key material in a way he felt was quasi-safe.
           - Until the "Internet-in-a-box" or TIA-type products are more
              widespread, many people will be connecting home or office
              machines to other systems they don't control. (To put this
              in sharper focus: do you want your electronic money being
              run out of an account that your sysop and his friends can
              monitor? Not hardly. "Electronic purses," which may be
              smart cards, Newton-like PDAs, or dongle-like rings or
              pendants, are clearly needed. Another entire discussion.)
 
 7.14. The Future of PGP
   7.14.1. "Does PGP help or hurt public key methods in general and RSA
            Data Security Inc. in particular?"
           - The outcome is not final, but on balance I think the
              position of RSADSI is helped by the publicity PGP has
              generated. Users of PGP will "graduate" to fully-licensed
              versions, in many cases. Corporations will then use
              RSADSI's products.
           + Interestingly, PGP could do the "radical" things that
              RSADSI was not prepared to do. (Uses familiar to
              Cypherpunks.)
             - bypassing export restrictions is an example of this
             - incorporation into experimental digital cash systems
           - Parasitism often increases the rate of evolution. Certainly
              PGP has helped to light a fire under RSADSI.
   7.14.2. Stealth PGP
           - Xenon, Nik, S-Tools,
   7.14.3. "Should we work on a more advanced version, a *Really Good
            Privacy*?"
           - easier said than done...strong committment of time
           - not clear what is needed...
   7.14.4. "Can changes and improvements be made to PGP?"
           - I consider it one of the supreme ironies of our age that
              Phil Zimmermann has denounced Tom Rollins for making
              various changes to a version of PGP he makes available.
           + Issues:
             - Phil's reputation, and that of PGP
             - intellectual property
             - GNU Public license
             - the mere name of PGP
             - Consider that RSA said much the same thing, that PGP
                would degrade the reputation of public key (esp. as Phil
                was an "amateur," the same exact phrasing PRZ uses to
                criticize Tom Rollins!)
           - I'm not taking a stand here....I don't know the details.
              Just some irony.
 
 7.15. Loose Ends
   7.15.1. Security measures on login, passwords, etc.
           - Avoid entering passwords over the Net (such as in rlogins
              or telnets). If someone or some agent asks for your
              password, be paranoid.
           - Can use encrypted telnet, or something like Kerberos, to
              avoid sending passwords in the clear between machines. Lots
              of approaches, almost none of them commonly used (at least
              I never see them).
