# Intro

The equivalent of hurting yourself in programming before you get to the heavy weights is writing unclean code. Unclean code is a lot of things. Ask any developer, and they’ll have a lot to say.

- code we can’t understand

- code that makes it hard to find what we’re looking for

- code that’s poorly formatted, untestable, and inflexible

- code that you and your team are afraid to change

- expensive

## Developer mindset

- Understand what makes programing a trade, the goals behind the software craftsmanship code of honor, and why we need a standardized set of ways to build software

- Produce better designs by cultivating a growth mindset, utilizing positive and negative feedback effectively, and acknowledging imperfections as growth opportunities.

- Learn how to increase the discoverability of your designs with the essential humancentered design principles traditionally only used by UX designers.

## Clean coding conventions

- Learn how to decode requirements, plan a project, and provide increasingly accurate estimates (maintainability, testability, flexibility).

- Learn formatting & style best practices (maintainability).

- Learn how to write useful comments and when to avoid writing comments(maintainability).

- Learn how to name things(maintainability).

- Learn how to organize things(maintainability).

- Learn how to prevent ilegal error states and elegantly handle errors and exceptions(maintainability).

- Learn testing approaches(testability).

- Learn architecture basics and designing to accomodate future changes(flexibility, maintainability).

- Learn to safely and effectively refactor code(maintainability).

## Skills & knowledge

- Learn why the only major innovation left in software design in tooling.

- Learn the essential tooling you need to have in your developer toolbox as a full-stack developer.

- Learn how to determine if you're dealing with absolute complexity or relative complexity.

- Learn how to detect code smells & anti-patterns.

- Learn when to optimize code.

## Understanding clean code

I’ve heard clean code described as plainly as when “everything is organized nicely”. I’ve heard it take a more opinionated form as “code with tests”. And I’ve heard it referred to as everything else in between.

Clean code is, in part, about code cleanliness. It is about following best practices, making code readable, and writing it so that every positive structural and stylistic trait you can assign to a codebase is evident.

Even as exhaustive as that sounds, it still barely scrapes the surface. The term, clean code, is incredibly overloaded.

### Clean code is an overloaded term

We expect clean code to be readable, understandable, flexible, testable, and maintainable. That's a lot to ask right off the bat. As a new or junior developer no being paid to write code in a professional setting, the process of learning how to write clean code is both daunting and somewhat nebulous.

It's daunting because your professional reputation rides on doing a good job, and it's nebulous because telling someone to write clean code is like telling someone to just run faster -- it's not easy to just start doing either of those things.

I'll introduce you to The Pillars of Clean Code:

1. Developer mindset

2. Coding convention

3. Skills & knowledge

Ultimately, you get your head right, develop a set of principled coding conventions, and improve them over time by learning the essential software design principles and patterns.

### What the community thinks about clean code

###### Community opinions

> Clean code is easy to read and modify, reveals the intended purpose without any obfuscation, and speaks a clear and consistent domain language.

###### My thoughts and comments:

- **Easy to read** could be a comment on naming things. It could also be a comment about how the code is physically styled and formatted to be easily read by humans.

- **Easy to modify** could be a comment on code being able to refactor code withour breaking it.

- **Reveals the intended purpose** could mean the names of the classes, methods, functions, and variables are so understandable that they couldn't be named any better.
  
  > Clean code is easy to read. It also has no coupling between libaries.

###### My thoughts and comments:

- Human readibility is undoubtedly one of the most important considerations. In the `coding conventions section`, we discuss human-centered-design and explore what makes code readable and what doesn't.

- The second comment is fascinating. It points to something more architectural. Admitedly, it's a bit of a rabbit hole - but they're right. `Coupling, packaging, depencency inversion, separation of concerns, and decomposion.` These are all about enforcing architectural boundaries and keeping dependencies at a distance. It’s funny. Coupling isn’t one of the first things you think about in the conversation of clean code, but it’s not to be excluded. The section about Skill & knowledge argues that being principled is what fosters better coding conventions. To me, this never ends. If you’ve got your Developer Mindset right, you’re always investing in your knowledge, picking up best practices, and learning ways to handle common problems in software development. For example, to keep libraries or modules decoupled, we, as an industry, have established well-known approaches to deal with this exact scenario. 

- Evolvable software. Change is a constant. We're always going to need to change code. So let's design it in a way to accomodate change.

- Telling the story of the domain menas that new developers can learn how the business works by reading the code. Code that encapsulates the essence of the business is desirable. in Chapter 5 - OOP & Domain Modeling, we learn how to separate the concerns of our app and carve out a domain model to build a codified version of the business. `I can read it without it being painful. I can change it without it breaking everything.`

- Readibility! Again! But also, ho do we write code that enables others to change it without breaking things? Tests, that is. Easier said than done! Inherently testable writing code isn’t obvious.
  
  Clean code is as much an art as a plumber installing a toilet, or an auto mechanic performing an oil change is. Clean code is code written `professionally`. The main them of professionalism ? Taking responsibility.
  
  > No magic. Simplicity
  
  This echoes simplicity over complexity. 
  
  - Sometimes the solutions is complicated because the problem is complicated. Accidental and Essential Complexity is a way to determine if the problem is difficult, or we make it difficult.
    
    > KISS, DRY, YAGNI, POLA, DIP, ideally facilitated by TDD
  
  Keep it simple, silly, Do Not Repeat Yourself, You Aren't Gonna Need It, Principle of Least Astonishment, Dependency Inversion Principle, and good ol' Test-Driven Development. This is definitely some design principle-soup. But honestly, if you know what each of these are, even if you choose not to follow 'em, having them in the back of your mind while coding can improve the structural quality of your designs.
  
  > Easily replaceable
  
  How do you design code to be replaceable ? By making it simple, readable, and providing tests. Using SOLID principles also helps.

###### What the experts think about clean code

> The cost of ownership for a program includes the time humans spend to understand it. Humans are costly, so ooptimize for understandability. - Mathias Verraes

> Code is like humor. When you have to explain it, it's bad. - Cory House

> Clean code always looks like it was written by someone who cares. There is nothing obvious you can do to make it better. - Michael Feathers

> Programming is the art of telling another human what one wants the computer to do - Donald Knuth

> If you want your code to be easy to write, make it easy to read - Robert C.Martin

Isn't it fascinating that most of the opinions about clean code from the experts have more to do with humans than they do about the code ? Call it chance, but these folks have spent decades doing this stuff.

###### How does unclean code get written ?

**When we try to go fast with arbitrary deadlines and really need more time.** Have you ever done anything well being rushed ? When we skip out on planning and estimation or find ourselves needing more time for whatever reason, instead of pushing back, we rush to tie up loose ends. This usually results in suboptimal, and unclean code.

**When we don't write tests.** Code without tests is code that cannot be refactored or changed safely. Since more time is spent on maintenance and improvement than on initial development, and change is always a constant factor, we need to feel like we can change code safely. Code unable to be changed safely induces unnecessary stress and anxiety. It also introduces risk. Code without tests is bad for your sanity, and it’s certainly not clean.

**When we don't care about the domain.** I can admit to this one. Sometimes you just really don't give a s**t about the project you're working on. It's less likely the next person will be able to maintain the code if we don't care about the domain, and the names don't reflect the business. Language is a huge part of software development. Not only might names be bad but code ends up in the wrong place, abstractions get missed, architectural boundaries are illegally crossed, and things inevitably become a mess.

**When we don't care about the longevity of a project.** To some, programming is just something you do for a paycheck. Maybe you got pinched throwing together a website for your aunt. Let's get it done, and get the hell out, right? That's a very irresponsible way to look at your job.

**When we don't care about craftmanship.** When we don't care about craftsmanship, a mess that works is acceptable. When we don't care about craftmanship, we won't challenge our perrs' code with constructive criticism. Potential conflict is scary, and people that don't care about craftmanship won't figure out ways to have productive discussions.

**When we're too scared to have design discussions with other developers.** It's realy unfortunate, because some of the best design decisions I've ever made came from more than one developer's point of view. Through tools like Slack, GitHub, and Jira, we can build collaboration into the process of developing software - but it takes will-power.

**When we try to get clever with our code.** What didn't make me feel cool and clever was watching my teammates avoid the code I wrote because they couldn't understand it. Writing clean code often means avoiding finesse, even when it's fun to do so.

**When our design skills are poor.** Design dictates if the project can endure or not: and design relies on empathy, a basic understanding of the psychology behind how we learn how to use things, and how to make things discoverable and understandable. They ain't teachin' that in school, bub.

**When systemic issues in the way we educate developers exists.** We live in a society that prefers to take a reactive approach to dealing with problems rather than a preventative one. Like most politics, a lasting change to this problem is hard and straighforward ways to fix them in the real-world don't exist. If developers are making messes in production codebases, potential ways to fix it are to: a) invest in better onboarding and training, b) educate developers with practical coding skills in post-secondary education and boot-camps, c) standardize practical coding skills instead of new technologies.

> These are some of the main ways unclean code gets written. Long story short, it's about people.

## Why It's hard to learn clean code

### Reason I - Humans are complex

Clean code has been hard to describe, learn, and teach because it aims to bring structure around `writing code for humans`, and humans are complex.

The human brain is still very much a big mystery to us. For example, we don't understand jack about how the brain processes **visual information**(AllenInstitute.org).

### Reason 2 - It's hard to deconstruct human psychology

While we can apply *reductionism* to computing and engineering, trying to do the same with humans is hard(and almost always wrong). This is likely why formal education has chosen to avoid attempting to teach us the following topics:

- How to name things

- How to organize code

- How to decide on and enforce coding convention

- How to detect code smells

- How to avoid anti-patterns

Designers learn the basics of human psychology, but traditionally, *software developers* don't. 

### Reason 3 - Trade skills are acquired through mentorship

They excel at teaching us scientific and theoretical aspects of computer science; but that's because they consider modern programming to be a **science** or engineering discipline, not a **trade**

The practical **tricks of the trade**; the things you'll spend 90% of your time doing in the real-world, like testing, refactoring, and design, are passed down to us. These learnings are passed down in apprenticeships, online training, co-ops, or junior development jobs with access to mentors and more experienced developers.



## The tree pillars of clean code

The Pillars of CLean Code is a framework I developed to illuminate each component involved in learning to write clean code. It breaks into three parts:

1. Developer mindset
   
   Professionalism, growth from failure, and design thinking.

2. Coding conventions
   
   Developing your own set of principled coding conventions to produce the highest quality software possible using industry standards, tools, approaches, and methods.

3. SKills & knowledge
   
   Become wise. Refine your preferred coding conventions from your skills(new languages, tooling, frameworks) and knowledge(design patterns, principles, approaches, experience, and judgment).
   
   
