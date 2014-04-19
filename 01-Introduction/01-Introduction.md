Introduction
============

## 1.1 Copyright

THE  CYPHERNOMICON: Cypherpunks FAQ and More, Version 0.666, 1994-09-10, Copyright Timothy C. May. All rights reserved. See the detailed disclaimer. Use short sections under "fair use" provisions, with appropriate credit, but don't put your name on my words.
  
## 1.2 Foreword

- The Cypherpunks have existed since September, 1992. In that time, a vast amount has been written on cryptography, key escrow, Clipper, the Net, the Information Superhighway, cyber terrorists, and crypto anarchy. We have found ourselves (or _placed_ ourselves) at the center of the storm.
- This FAQ may help to fill in some gaps about what we're about, what motivates us, and where we're going. And maybe some useful knowledge on crypto, remailers, anonymity, digital cash, and other interesting things.
- The Basic Issues
  - Great Divide: privacy vs. compliance with laws
    - free speech and privacy, even if means some criminals cannot be caught (a stand the U.S. Constitution was strongly in favor of, at one time)
      - a man's home is his castle...the essence of the Magna Carta systems...rights of the individual to be secure from random searches
    - or invasive tactics to catch criminals, regulate behavior, and control the population
      - the legitimate needs to enforce laws, to respond to situations
    - this parallels the issue of self-protection vs. protection by law and police
      - as seen in the gun debate
      - crypto = guns in the sense of being an individual's preemptive protection
    - past the point of no return
  - Strong crypto as building material for a new age
  + Transnationalism and Increased Degrees of Freedom
    - governments can't hope to control movements and communications of citizens; borders are transparent
+ Not all list members share all views
  - This is not "the Official Cypherpunks FAQ." No such thing can exist. This is the FAQ I wanted written. Views expressed are my own, with as much input from others, as much consensus, as I can manage. If you want a radically
 different FAQ, write it yourself.  If you don't like this FAQ, don't read it. And tell your friends not to read it. But don't bog down my mailbox, or the 500 others on the list, with messages about how you would have worded Section 12.4.7.2 slightly differently, or how Section 6.9.12 does not fully reflect your views. For obvious reasons.
  - All FAQs are the products of a primary author, sometimes of a committee. For this FAQ, I am the sole author. At least of the version you are reading now. Future versions may have more input from others, though this makes me nervous (I favor new authors writing their own stuff, or using hypertext links, rather than taking my basic writing and attaching their name to it--it is true that I include the quotes of many folks here, but I do so by explicitly quoting them in the chunk they wrote....it will be tough for later authors to clearly mark what Tim May wrote without excessively cluttering the text. The revisionist's dilemma.
  - The list has a lot of radical libertarians, some anarcho-capitalists, and even a few socialists
  - Mostly computer-related folks, as might be expected. (There are some political scientists, classical scholars, etc. Even a few current or ex-lawyers.)
  + Do I Speak for Others?
  + As I said, no. But sometimes I make claims about what "most" list members believe, what "many" believe, or what "some" believe.
  - "Most" is my best judgment of what the majority believe, at least the vocal majority in Cypherpunks discussions (at the physical meetings, parties, etc.) and on the List. "Many" means fewer, and "some" fewer still. "A few" will mean a distinct minority. Note that this is from the last 18 months of activity (so don't send in clarifications now to try to "sway the vote").
  - In particular, some members may be quite uncomfortable being described as anarchists, crypto anarchists, money launderers, etc.
+  My comments won't please everyone
  - on nearly every point ever presented, some have disagreed
  - feuds, battles, flames, idee fixes
  - on issues ranging from gun control to Dolphin Encrypt to various pet theories held dearly
  - Someone once made a mundane joke about pseudonyms being like multiple personality disorder--and a flame came back saying: "That's not funny. I am MPD and my SO is MPD. Please stop immediately!"
  - can't be helped....can't present all sides to all arguments
+ Focus of this FAQ is U.S.-centric, for various reasons
  - most on list are in U.S., and I am in U.S. 
  - NSA and crypto community is largely centered in the U.S., with some strong European activities
  - U.S. law is likely to influence overseas law
+ We are at a fork in the road,  a Great Divide
  - Surveillance vs. Freedom
  - nothing in the middle...either strong crypto and privacy is strongly limited, or the things I describe here will be done by some people....hence the "tipping factor" applies (point of no return, horses out of the barn)
+ I make no claim to speaking "for the group." If you're offended, write your own FAQ. My focus on things loosely called "crypto anarchy" is just that: my _focus_. This focus naturally percolates over into something like this FAQ, just as someone primarily interested in the mechanics of PGP would devote more space to PGP issues than I have.
  - Gary Jeffers, for example, devotes most of his "CEB" to issues surrounding PGP.
+ Will leave out some of the highly detailed items...
  - Clipper, LEAF, escrow, Denning, etc.
  - a myriad of encryption programs, bulk  ciphers, variants on PGP, etc. Some of these I've listed...others I've had to throw my hands over and just ignore. (Keeping track of zillions of versions for dozens of platforms...)
  - easy to get lost in the details, buried in the bullshit
  
## 1.3 Motivations

- With so much material available, why another FAQ?
- No convenient access to archives of the list....and who could read 50 MB of stuff anyway?
- Why not Web? (Mosaic, Http, URL, etc.)
- Why not a navigable Web document?
- This is becoming trendy. Lots of URLs are included here, in fact. But making all documents into Web documents has downsides.
+ Reasons why not:
  - No easy access for me.
  - Many others also lack access. Text still rules.
  - Not at all clear that a collection of hundreds of fragments is useful
  - I like the structured editors available on my Mac (specifically, MORE, an outline editor)
- What the Essential Points Are
  - It's easy to lose track of what the core issues are, what the really important points are. In a FAQ like this, a vast amount of "cruft" is presented, that is, a vast amount of miscellaneous, tangential, and epiphenomenal material. Names of PGP versions, variants on steganograhy, and other such stuff, all of which will change over the next few months and years.
  + And yet that's partly what a FAQ is for. The key is just not to lose track of the key ideas. I've mentioned what I think are the important ideas many times. To wit: 
    - that many approaches to crypto exist
    - that governments essentially cannot stop most of these approaches, short of establishing a police state (and probably not even then)
    - core issues of identity, authentication, pseudonyms, reputations, etc.

## 1.4 Who Should Read This
- "Should I read this?"
    - Yes, reading this will point you toward other sources of
      information, will answer the most commonly asked questions,
      and will (hopefully) head off the reappearance of the same
      tired themes every few months.
   - Use a search tool if you have one. Grep for the things that
      interest you, etc. The granularity of this FAQ does not
      lend itself to Web conversion, at least not with present
      tools.
   + What _Won't_ Be Covered Here
     + basic cryptography
     + many good texts, FAQs, etc., written by full-time
      cryptologists and educators
        - in particular, some of the ideas are not simple, and
            take several pages of well-written text to get the
            point across
               - not the focus of this FAQ
         - basic political rants
  
## 1.5. Comments on Style and Thoroughness
- "Why is this FAQ not in Mosaic form?"
   - because the author (tcmay, as of 7/94) does not have Mosaic
      access, and even if did, would not necessarily....
   - linear text is still fine for some things...can be read on
      all platforms, can be printed out, and can be searched with
      standard grep and similar tools
- "Why the mix of styles?"
   + There are three main types of styles here:
     - Standard prose sections, explaining some point or listing
       things. Mini-essays, like most posts to Cypherpunks.
     + Short, outline-style comments
       - that I didn't have time or willpower to expand into
       prose format
       - that work best in outline format anyway
       - like this
     + Quotes from others
       - Cypherpunks are a bright group. A lot of clever things
       have been said in the 600 days x 40 posts/day = 24,000
       posts, and I am trying to use what I can.
       + Sadly, only a tiny fraction can be used
        - because I simply cannot _read_  even a fraction of
            these posts over again (though I've only saved
            several thousand of the posts)
        - and because including too many of these posts would
            simply make the FAQ too long (it's still too long, I
            suppose)
           - I hope you can handle the changes in tone of voice, in
              styles, and even in formats. It'll just too much time to
              make it all read uniformly.
- Despite the length of this thing, a vast amount of stuff is
    missing. There have been hundreds of incisive analyses by
    Cypherpunks, dozens of survey articles on Clipper, and
    thousands of clever remarks. Alas, only a few of them here.
   - And with 25 or more books on the Internet, hundreds of FAQs
      and URLs, it's clear that we're all drowning in a sea of
      information about the Net.
   - Ironically, good old-fashioned books have a lot more
      relevant and timeless information.
      
- Caveats on the completeness or accuracy of this FAQ
    + not all points are fully fleshed out...the outline nature
      means that nearly all points could be further added-to,
      subdivided, taxonomized, and generally fleshed-out with
      more points, counterpoints, examples
     - like a giant tree...branches, leaves, tangled hierarchies
    + It is inevitable that conflicting points will be made in a
      document of this size
     - views change, but don't get corrected in all places
     - different contexts lead to different viewpoints
     - simple failure by me to be fully consistent
     - and many points raised here would, if put into an essay
        for the Cypherpunks list, generate comments, rebuttals,
        debate, and even acrimony....I cannot expect to have all
        sides represented fully, especially as the issues are
        often murky, unresolved, in dispute, and generally
        controversial
    - inconsistencies in the points here in this FAQ
  
## 1.6. Corrections and Elaborations
 + "How to handle corrections or clarifications?"
   - While I have done my best to ensure accuracy, errors will
      no doubt exist. And as anyone can see from reading the
      Cypherpunks list, nearly *any* statement made about any
      subject can produce a flurry of rebuttals, caveats,
      expansions, and whatnot. Some subjects, such as the nature
      of money, the role of Cypherpunks, and the role of
      reputations, produce dozens of differing opinions every
      time they come up!
   - So, it is not likely that my points here will be any
      different. Fortunately, the sheer number of points here
      means that not every one of them will be disagreed with.
      But the math is pretty clear: if every reader finds even
      one thing to disagree with and then posts his rebuttal or
      elaboration....disaster! (Especially if some people can't
      trim quotes properly and end up including a big chunk of
      text.)
+ Recommendations
 - Send corrections of _fact_ to me
 - If you disagree with my opinion, and you think you can
    change my mind, or cause me to include your opinion as an
    elaboration or as a dissenting view, then send it. If
    your point requires long debate or is a deep
    disagreement, then I doubt I have the time or energy to
    debate. If you want your views heard, write your own FAQ!
 - Ultimately, send what you want. But I of course will
    evaluate comments and apply a reputation-based filter to
    the traffic. Those who send me concise, well-reasoned
    corrections or clarifications are likelier to be listened
    to than those who barrage me with minor clarifications
    and elaborations.
 - In short, this is not a group project. The "stone soup
    FAQ" is not what this is.
    
+ More information
     - Please don't send me e-mail asking for more information
        on a particular topic--I just can't handle custom
        research. This FAQ is long enough, and the Glossary at
        the end contains additional information, so that I cannot
        expand upon these topics (unless there is a general
        debate on the list). In other words, don't assume this
        FAQ is an entry point into a larger data base I will
        generate. I hate to sound so blunt, but I've seen the
        requests that come in every time I write a fairly long
        article.
   + Tips on feedback
     - Comments about writing style, of the form "I would have
        written it _this_ way," are especially unwelcome.
 + Credit issues
   - inevitable that omissions or collisions will occur
   - ideas have many fathers
   - some ideas have been "in the air" for many years
   + slogans are especially problematic
     - "They can have my...."...I credit Barlow with this, but
        I've heard others use it independently (I think; at least
        I used it before hearing Barlow used it)
     - "If crypto is outlawed, only outlaws will have crypto"
     - "Big Brother Inside"
   - if something really bothers you, send me a note
  
## 1.7. Acknowledgements
- Acknowledgements
   - My chief thanks go to the several hundred active
      Cypherpunks posters, past and present.
   - All rights reserved. Copyright Timothy C. May. Don't try to
      sell this or incorporate it into anything that is sold.
      Quoting brief sections is "fair use"...quoting long
      sections is not.
  
## 1.8. Ideas and Notes (not to be printed)
- Graphics for cover
   - two blocks...plaintext to cryptotext
   - Cypherpunks FAQ
   - compiled by Timothy C. May, tcmay@netcom.com
   - with help from many Cypherpunks
   - with material from other sources
   - <credited in angle brackets>
   - "So don't ask"
  
## 1.9. Things are moving quickly in crypto and crypto policy
- hard to keep this FAQ current, as info changes
- PGP in state of flux
- new versions of tools coming constantly
- And the whole Clipper thing has been turned on its head
    recently by the Administration's backing off...lots of points
    already made here are now rendered moot and are primarily of
    historical interest only.
   - Gore's letter to Cantwell
   - Whit Diffie described a conference on key escrow systems in
      Karlsruhe, Germany, which seemed to contain new ideas
   - TIS? (can't use this info?)
 
## 1.10. Notes: The Cyphernomicon: the CypherFAQ and More
 - 2.3.1.  "The Book of Encyphered Names"
   - Ibn al-Taz Khallikak, the Pine Barrens Horror.
   - Liber Grimoiris....Cifur???
   - spreading from the Sumerian sands, through the gate of
      Ishtar, to the back alleys of Damascus, tempered with the
      blood of Westerners
   - Keys of Solomon, Kool John Dee and the Rapping Cryps  Gone
      to Croatan
   - Peter Krypotkin, the Russian crypto anarchist
   - Twenty-nine Primes, California
- 2.3.2.  THE CYPHERNOMICON: a Cypherpunk FAQ and More---
            Version 0.666
- 1994-09-01,   Copyright Timothy C. May,   tcmay@netcom.com

           - Written and compiled by Tim May, except as noted by
              credits. (Influenced by years of good posts on the
              Cypherpunks list.) Permission is granted to post and
              distribute this document in an unaltered and complete
              state, for non-profit and educational purposes only.
              Reasonable quoting under "fair use" provisions is
              permitted. See the detailed disclaimer of responsibilities
              and liabilities in the Introduction chapter.
