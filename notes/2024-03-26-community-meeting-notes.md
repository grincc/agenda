# Community Meeting Notes March 26, 2024

Community Council (CC) meeting held in grincoin#general channel keybase chat. Meeting duration not explicitly stated, but inferred to be between 45-60 minutes.

Notes are truncated, and conversations sorted based on topic and not always chronological. Quotes are edited for brevity and clarity, and not always exact.

### _Community attendance:_

* anynomous
* yeastplume
* i1skn

# Short Summary

-  Update on the development status of the Grin GUI wallet, particularly issues related to updating the `iced-rs` library.
-  Discussion on the challenges of working with `iced-rs` and its lack of maturity, and potential benefits once this update is completed.
-  Comparison of the programming languages Rust, Python, and JavaScript, and their suitability for different tasks.

# Agenda Points & Actions

*   No explicit agenda was stated.
*   Update on the development status of the GUI wallet.

## Grin GUI Wallet Development

__anynomous__: @yeastplume Any news on the development of the GUI wallet?

__yeastplume__: Sure, I'm doing tons of work on it at the moment, but it's all going backwards :D

__anynomous__: backwards? I see I am one version behind, I am still testing alpha-5

__yeastplume__: What I mean is I'm updating `iced-rs` to the latest version, and it's been the most painful update so far, it's taken days to get it to compile.

__anynomous__: auch. Kind of hard being one of the alpha testers of Iced. Is getting to maturity you think?

__yeastplume__: It is compiling now, but some custom widgets I had for displaying tables aren't working at the moment, and I need to figure out why or possibly see if anyone else has created any table widgets anywhere. Once this is done we should get some benefits, text areas being one which means we can input seed phrases properly.

__anynomous__: Perhaps best to try to merge those widgets into Iced, in the hope they will get long term support, or get tested and fixed with new releases. This sounds like something they should add to Iced for sure.

__yeastplume__: I think the problem is that it's one person working on it… I mean he's working hard on it but he's a bit of a soloist and doesn't seem to care how many changes and reworks things or what it breaks. I don't think that project will start seeing anything resembling maturity until a proper governance team develops around it.

__anynomous__: For that he probably needs a few more projects to use his code and start screaming when he kills backwards compatibility with reworks.

__yeastplume__: right now he does what he wants, it's very difficult to find information on what changed between versions and why (other than inadequate auto-generated lists.) so you have to dig through the repo history to possibly find out what needs to be updated. So, it's frustrating in that regard.

__anynomous__: That does sound difficult…

__yeastplume__: But, it's Rust!

__anynomous__: Yes, it is! In the long term I am sure taking the hard/high rode will pay off. But for the moment it means the road ahead will be more difficult and frustrating. I have to get back to learning Rust myself, but I have to admit it is a bit hard without having a direct project that depends on it.

__yeastplume__: I kind of do as much as I can in Rust now, I'd even prefer in places where people might normally use scripting languages… all the libs around it are so good at parsing, transforming, serializing, all sorts of things, but I digress

## Programming Languages Discussion

__anynomous__: Personally I use Python where I can with wrapped Rust libraries, since their performance just blows me away. Often way faster than similar libraries compared to Python native libraries, it can easily be a factor 10-100 times faster. What I really do not understand is people using JavaScript, since in that case Python is even way faster as well as easier to read than similar code in JavaScript.

__yeastplume__: I think a lot of people just know javascript so they use it

__anynomous__: Probably, and yes, easy for web integration. But most libraries are horrible in my opinion. The only use I have for them is to read for example wallet code in javascript and reimplement them in Python with much performance gains.

__yeastplume__: yeah, the dependencies to pull in for every tiny lib are horrendous, and they're mostly unaudited, unvalidated or anything

__anynomous__: Exactly, sometimes even hard to reproduce in Python because they contain hidden bugs.

__yeastplume__: which is why we're not using it for the wallet gui, even though it would be simpler

__anynomous__: Again, I am sure that on the long run that will pay off. I just hope one day I will be as good with Rust as I am with Python so I can use its full potential.

__i1skn__: I hope one day Rust would be good for UI as other languages, would be super cool to do UI in Rust

__anynomous__: Absolutely. For now it is a pain, but Rust is expanding in all directions, so it is only a matter of time for some mature libraries to appear.

## *TO DO List*

*  @yeastplume: Continue updating `iced-rs` library for the GUI wallet and address the custom widget issues.


**Meeting adjourned.**