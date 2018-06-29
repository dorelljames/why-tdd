<!-- https://www.slideshare.net/bmabey/the-why-behind-tddbdd-and-the-how-with-rspec?qid=5e143253-b892-43c3-8c3f-8024ead828a7&v=&b=&from_search=5 -->

class: middle, center
# "Why Test and why TDD?"
Laravel Cebu &middot; Meetup for May &middot; June 3, 2017 @ Codigu, Inc.

---

class: middle, left
# # whoami

---

class: middle, left
# Dorell James Galang

--

- Role: Offlane

- MMR: 2k scrubz...

- Motto: Life is a game of luck.

- Friend ID: 11875883

---
class: middle, left

# Dorell James Galang

- Role: Full Stack Developer

- Status: Single, ready to mingle... :P

- Motto: YOLO but once is enough if you do it well...

- Contact: dorelljames.com

???
Before we begin, I want you all to reflect on this following questions and see if it sounds true to you because at the end of the day, we'll try to change and improve things here. I'm not saying that what we're going to talk today is the best out there but I assure to you all, your life as a developer/programmer will never be the same once you do this.

---

class: middle, left
# What is Testing to you?

--

- Ensuring code does what it is meant to do

--

- Ensuring system works as expected

--

- Being able to manually test things

---

class: middle, left
# What is your current testing strategy?

--

- Code and hope it works?  

--

- Code locally, test, push to production and retest?  

--

- Staging Environments?

---


class: middle, center
# Why do we test?

???
Did any of those are actually part of your reality?

It is important that we take a look at what and how we're doing things to go forward and understand why we probably need change. After all, who doesn't want to improve?
---

class: middle, center
## 1. Confidence.
???
It is by verification that our system behaves as it is suppose to. Software testing enables making objective assessments regarding the degree of conformance of the system to stated requirements and specifications.

--

class: middle, center
## 2. Validation.
???
Testing validates that the system being developed is what the user needs. In essence, validation is performed to ensure that we are building the right system. Apart from helping make decisions, the information from software testing helps with risk management.

--

class: middle, center
## 3. Quality / Bugs
???
Finding defects / bugs is one of the purposes of testing, it is not the sole purpose. It is important for testing to verify and validate that the product meets the stated requirements / specifications which in return reduce post release costs of support and service, while generating customer good will that could translate into greater revenue opportunities.


---

class: middle, center
# Manual or Automated?
Automation is clearly our friend.

???
I challenge you all whether you are a newbie, an average programmer or a rockstar to release the inner geek of you and do test. Who doesn't test by the way? Automation is great because "we are lazy", aren't we? Joking aside, it's not our primary job to test but writing tests puts us into a state of "high level" confidence which also in return makes us proud of our work.
---

class: middle, center
# "Good code makes a happy programmer. A good programmer makes good code. :)"
???
Who said that? Don't ask, I just make that shit but it sounded right so I might as well include it. :D

---

class: middle, center
# Why automation?
---

class: middle, center
## 1. Confidence. Regression tests!

???
It's funny I'm talking about this "regression tests" now while nobody cared to explain to us what it's all about and I'm doing that for almost 3 years way back on my NCR years. Anyhow, thank me later 'coz you don't have to wait 3 years to know what is it all about. In a nutshell, all it does is that it verifies that software which was previously developed and tested still performs correctly after it was changed or interfaced with other software. Changes may include improvements, bugfixes, other integrations, etc.

--

## 2. Refactoring. Shortened feedback loop.

???
Improving code. Shortened feedback loop makes improving our design much easier and less painful. The process not only makes you design your code well and captures bug but it most likely force you to keep things really simple


---
class: top, center
# Riddle me this...
Which tests instill more confidence of a system's behavior in you?  
(Assume they have the same coverage)


--

### ▢ Tests written after functionality is added.

--

### ▢ Tests written before functionality is added.

--

# ✓ Neither. Both provide equal confidence.

---

class: middle, center
# But why test first?

--

- Most of us aren't disciplined enough to test last. Once we have manually tested the system taking the time write an automated test seems like a pain.

???
There it goes again, the "lazy programmer" comes in. 

--

- Code that isn't written with tests in mind tends to be very difficult to test without refactoring it first.

???
When you write code with focus on user end functionality, we tend to forget to design it well. And when a bunch of things are tightly coupled and depends a lot of on each other, refactoring is so hard, much more testing each unit and the smaller parts.

---

class: middle, center
# Clear up a common misconception...

---

class: middle, center
### TDD !== writing tests first

---

class: middle, center
## TDD =~ writing tests first... but

---

class: middle, center
## TDD isn't about testing...

---

class: middle, center
# TDD is about DESIGN

--

### <a style="color: red;">RED</a> -> <a style="color: green;">GREEN</a> -> <a style="color: orange">REFACTOR</a>

---

class: middle, center
# Design is a <strong>PROCESS</strong> not a <strong>PHASE</strong>

--

The TDD cycle of <a style="color: red;">RED</a> -> <a style="color: green;">GREEN</a> -> <a style="color: orange">REFACTOR</a> enables you to iterate over your design constantly by removing duplication (refactoring). Testing units in isolation allows you to achieve high cohesion and loose coupling regularly.

???
I am sure to those who are doing TDD, they can really relate to this so well. Often, they're really confident programmers as they are somehow ensured that their work is properly documented, tested, etc.

---

class: middle, left
# Side benefits of TDD are...

--

- Verification of behavior.

???
next

--

- Documentation.
???
next

--

- Confidence.
???
next

---

class: middle, center
## "The act of writing a unit test is more of an act of design than of verification. It is also more of an act of documentation than of verification. The more act of writing a unit test closes a remarkable number of feedback loops, the least of which is the one pertaining to verification of function." 

-- "Uncle" Bob Martin

---
class: top, center
# Riddle me that...
Which tests instill more confidence of a system's deisgn and long term maintainability?

--

### ▢ Tests written after functionality is added.

--

### ▢ Tests written with good TDD skillzzz.

--

# ✓ It depends. Are you "Bob Martin" or Adam, Jeff or even Taylor? :P

--

But actually, I'm with the latter here. Only when "TDD" is done right...

---

class: top, left
# Wrapping things up.

- TDD != writing tests first... and not certainly just "testing". It's a DESIGN process.

- Always remember, <a style="color: red;">RED</a> (failing tests) -> <a style="color: green;">GREEN</a> (success tests) - <a style="color: orange;">REFACTOR</a> (improving code) cycle.

- In result, it gives us confidence that our system behaves the way it's supposed to be.

- Lastly, it doesn't hurt to test manually but it makes a programmer happy to "automate" testing and be so much confident with the quality of our work.

- For further learning, read about "BDD".

