---
title: "What is (true) Shift Left in Security?"
date: 2023-1-1
draft: false
description: "Post on what is real shift left"
summary: "A post to understand what a true shift left is."
slug: "shiftleft"
---
> ### KEY TAKEAWAYS:
> - Security Automation and integration into dev pipelines are great but not sufficient.
> - Most of us are playing a never-ending game.
> - A true Shift left is shifting left to the origin of the problem.

You probably have heard the term Shift Left with respect to software security. 

Many of us understand this as performing security related tasks much earlier in the software life cycle. 
Some of those tasks include having Continuous Integration (CI) with security tools and automatically scanning and testing the builds on every new change, etc. Though this is good practice and gives the product teams faster security feedback, a true Shift left is much more.

If you are thinking about achieving true product security across the board, then this security automation and integration alone is not sufficient. <br>
Couple of reasons: 
1.	Automated security tools alone will NOT uncover all software weaknesses. 
2.	Secondly, these security practices are basically helping to find security issues early, however, they are not preventing these security issues from coming again. <br>
In other words, this is a never-ending game.

So, a real shift left means to shift left as close as possible to the point where the security issues are introduced and then try to stop them right there. <br>
If you have not guessed it already, that point is when the code is being written by the developers.

So you ask,
 - What do I mean by shift left to the developers? <br>
 - Am I talking about running static analysis on the code while it is being written? <br>

Well, No. I am not talking about any automation here.

It is basically the humans (every engineer) that write, review and test code need to be educated to stop introducing the security issues at first place. <br>

In my close to 2 decades of security practice/experience, most (not all) of the vulnerabilities that I have come across, **I strongly believe** they could have been found by the primary developer him/herself OR the secondary developer who reviewed and approved the code, period. <br>
I really mean this by my first-hand experience and not exaggerating here. 

Am I now saying every engineer should be a security engineer? <br>
No, that’s not what I meant and practically that is not possible too.

What I meant and is something I believe **achievable** is every engineer must be a **security aware** and a **security minded** individual.

 - A security aware engineer is one who is aware of the most common vulnerabilities out there. He/she doesn’t need to be a security expert but just be aware of WHAT. 
 - A security minded engineer is one who thinks, questions, and apply security at every stage of software building. <br>
 He/she again doesn’t need to be a security expert for this, but someone capable of asking the right questions (which is learnable and sometimes come naturally if you apply your thoughts or be in the right environment that fosters security).

So how do we make every engineer a security aware and security minded individual? <br>
Well, it’s not as easy as just simply having all the Engineers go through some yearly security training materials.

It’s a cultural shift that needs to happen, if not across the company, at least within a product organization.

So how do we get there? <br>
Look out for my future part 2 of this article for some ideas I think we could implement to achieve this.