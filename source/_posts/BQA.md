title: What lessons I learned as a Q-BA?
date: 2012-09-26
categories:
- Work
tags:
- BA
- QA
- Lessons Learned
comments: true
---

** Q-BA here is referring new BA who acted as a QA before, just like me...**

I acts as QA in the last two years, and although I tried to do some stuff related to business, however, it is slightly different when I acts as a full-time BA in the current project.

In one word, I think the difference is, as QA, I accept the fact that all the behaviors is well-considered and good enough, then the only think I need to check is if they are working well.

However, as BA, I think I should be more critical of the proposed option, and try to find if it is really suitable for the business needs.

### Lesson1: Does sad path really matter?

From QA perspective, especially when most of happy path is guaranteed by kinds of tests, then finding evil scenarios to break the application is really important in my QA career.

So at the beginning of the BA career, I always tend to find out all sad paths for the scenario.

**Example:**

**When** I am working on the story elaboration of one story" save and send email", which is about asking the user email, then send the product info to the user via email.

**Then**

**From QA perspective,**

I mainly focusing on handling the bad path, how about it is empty, how about if it is too long, how about if it is not well-formatted
	...

**From BA perspective,**

First thing is to see if it makes sense to ask user to input it again, how about pre-populate it since it is asked before? ...

### Lesson2: Do not be pulled into details too much!

From QA perspective, I did many scenario testing(system capability for user to achieve specific goal) and story testing(provide/get fast feedback along the story development process).

So I prefer to go to details as per each scenario, and try to evolve more detailed scenario.

Then from BA perspective, the whole part is more important than focusing on the small part and detailed information.

**Example:**

**Given** we are working on the project in the initiate phase

**When** prototype comes passed from Business to us for reference

**Then**

**From QA perspective,**

I mainly find flaws as per each section, and to check the text field and buttons behaviors.

I mainly find if any spelling errors around all the wording and text...

**From BA perspective,**

*[I need to think more like UX]*

Do we need to schedule user testing or expert review of the prototype to see if the design makes sense?

*[I need to think more like Dev]*

What's the integration points among the system with other systems?

If the wording and text need to be approved by legal team?...

### Lesson3: Go directly to the business for any need

From QA perspective, sometimes I will firstly go to BA if some puzzles happen.And then go to business if necessary.

Then from BA perspective, if any puzzle happen, go to the people you need to ask for answers. Don't Wait!

### Lesson4: Facilitation skills matter a lot

As a BA, the facilitation skill is important to gather the clarification and solution.

There are many scenarios you need to facilitate the meeting at the inception phase of the project, or during daily business discussion, IPM and meetings.

*I just realized the importance, and I think the book <the secret of Facilitation> is really cool, thanks kangkang's recommendation.*
