**Sable’s 3 groups of software products**

* Small to medium size products: more common 

    * few devs

    * development lasts few weeks to couple of years

    * Payment may be tens of thousands of $

    * customer small company or organization

* Large projects intended for mass use

    * involves many devs, proj managers, maybe over 100

    * devs last > 1yr , maybe 2-3

    * Cost to company is hundreds of thousands to millions

    * Customers are real people

    * each copy might be $$$ hundreds 

* Large project intended for single company or organization

    * involves many devs 

    * development lasts years

    * customer is a single company or organization

    * the customer pays hundreds of thousands or millions of dollars

    * contract negotiation

*In class, we discussed several types of software engineering projects. For which type is the maintenance phase the most important?*

Usually large projects intended for a single company/organization

**Maintenance  **

*Related to system maintenance, Lehman has defined three categories of software systems; namely, S-systems, P-systems, and E-systems.  Explain these categories.*

	S - systems ("static") formally defined (ex. matrix mult)

		do not easily accommodate changes to problems

	P - system ("practical") more dynamic, develops approximate solutions where feedback improves solutions over time- theoretically, there’s a complete solution, but we don’t know what it is (i.e. chess AI)

	E-system ("environment") embedded in the real world and affected by changes in real world and adapts. (i.e. piccadilly television- made to compete with cable and satellite, changes based on what’s available, what’s desired, communication laws, etc.)

 

*We have discussed several reasons that maintaining a software system can be difficult.  Name and define four.*

* The need to change system has to be balanced with the need to keep the system accessible (maintenance downtime)

* Maintainers may not understand the code

* Communication with (non-technical) users

* Pressure to make quick changes (not good changes)

* Low morale (lol)

* Illogical artifacts left over from legacy code

* Object-oriented code- complex interactions between parts

* Difficult to find time to continue proper testing

* Combinations of changes can introduce new faults

* Gunning’s Fog Index - readability measure

*W**e have discussed four types of tasks that maintainers of a software system spend their time on; name and define two.*

* Corrective maintenance -  bug fix/feature adding

* Adaptive maintenance - when you change something you have to change other things

* Perfective maintenance - change that improves some part of the program/system

* Preventative maintenance - make failures less likely in the future

*Relative to the past, why is maintenance such an important phase of the software life cycle today?*

	Once software is released and being used, the final phase of the cycle is to keep your customers happy and continue to maintain and support your software. Nowadays a lot more maintenance than dev.

*Assume that a company purchases your Set program and pays you to maintain it over time. At some point, they ask you to add information to the database related to users such that all users have a rating, and whenever a user wins or loses a game, their rating gets adjusted according to formulas specified by the company. You implement this change, but realize that there is nothing in the system that makes the information noticeable. You therefore change the user interface such that users can click on the usernames of their opponents, or potential opponents, to see their rating. When you make this change to the interface, what type of maintenance is this an example of?*

	Adaptive

**Lehman - Program Evolution**

*What is stated by Lehman's fundamental law of program evolution?*

Program evolution is subject to measurable trends of the extent it changes, becomes more complex, etc.

*In class, we mentioned that one metric for measuring code complexity is called the cyclomatic number (we did not actually define it). Which of Lehman's laws of program evolution says something about this metric, and what does it predict?*

Increasing complexity measures # of linearly independent paths in code: as the program changes and becomes more complex, its structure deteriorates. 

*We have discussed Lehman's five laws of program evolution; describe his five laws, what do they state, and can anything be done about it?*

* continuing change: programs have to continually change or will cease to be useful eventually

* increasing complexity causes deterioration (constant refactoring => prevents, but takes time + effort)

* fundamental law of program evolution - changes in programs and their complexities are predictable (measurable trends)

* Conservation + organizational stability - won’t suddenly experience changes - somewhat stable work rate in the long run

* Conservation of familiarity - complexity of change between releases is statistically nonexistent - step between changes becomes more insignificant

**Code quality **

*What has empirical evidence shown about the effects of reuse on code quality?*

*What have studies suggested about the effects of reuse on code quality?*

Studies have shown both that code reuse can increase the number of bugs if modified by 25% or decrease the number of bugs.

*In general, what has the software engineering literature shown about the effect of code inspections on code quality?*

They work very well. Catching most faults.

**Quality models**

*Related to the evaluation of software products, explain the notion of a quality model.*

A model/framework to determine what defines quality/evaluate the quality of software products by tying together different characteristics--shows how we measure quality, what we look for

*Related to the evaluation of software products, specify a problem with early quality models, such as McCall's or Boehm's, that later quality models attempted to correct.*

Each right hand quality only matches one left hand quality; focuses on user’s view of the software rather than developer’s

*What are quality models, such as Boehm's model or Dromey's model, used for?*

*What does the software engineering literature suggest about the effects of code inspections on code quality?*

*If a u-plot is consistently and significantly below the 45 degree line, what does this mean, specifically, about the predictions it makes related to failure times?*

This means that predictions are pessimistic because the software performs better that you predict ie predicted times to failure are lower that the actual times to failure.

*What will a u-plot look like if predictions are biased?*

It will either be consistently and significantly below or above the 45° line.  Above is optimistic, below is pessimistic.

*When deciding whether or not to believe the results of a published study, I have said that one thing you should consider is publication bias.  What does this refer to?*

Often people will only publish the results of a study if they get results that are unusual -- so you’ll only see the small minority of studies done that get that unusual result, but you won’t see papers on studies that got the standard result.

*Related to process maturity, what is the difference between the Capability Maturity Model and the People Capability Maturity Model?*

Capability Maturity Model evaluates and rates a software organization as a whole but doesn’t include ratings on how good the actual programmers there are

People Capability Maturity Model evaluates and rates the programmers of a software organization

*Without defining its levels, briefly describe the Capability Maturity Model and state its two main purposes.*

*Initial*  - the starting point for use of a new or undocumented repeat process.

*Repeatable* - the process is at least documented sufficiently such that repeating the same steps may be attempted.

*Defined* - the process is defined/confirmed as a standard business processes.

*Managed* - the process is quantitatively managed in accordance with agreed-upon metrics.

*Optimizing* - process management includes deliberate process optimization/improvement.

*Related to the evaluation of software organizations, what major factor was left out of the capability maturity model that a later maturity model attempted to incorporate?*

Evaluating how good the programmers are 

*Name one reason that some people are critical of the Capability Maturity Model.*

Doesn’t evaluate programmers

Surveys:

* Yes/no questions

* Voluntary

* Don’t know if people answer honestly

**Evaluating Products, Processes, Resources**

We have learned that four evaluation techniques used in the software industry are feature analyses, surveys, case studies, and formal experiments. Of these techniques, specify which ones, if any, can be applied retrospectively?

* Feature analysis

* Surveys → retrospective

* Case studies

* Formal experiments - what level of control you have over the variables, etc

* Statistical significance (publications may not be great)

Name one problem with the use of surveys to evaluate software engineering processes, as opposed to using case studies or formal experiments.

Name one problem with the use of surveys to evaluate software processes, tools, techniques, or products.

**Technology Transfer**

*According to a business school study related to technology transfer, what is the difference between innovators and early adapters? Related to technology transfer, what are laggards?*

Innovators 2.5% hipsters : first to try new things, for the sake of new technology

Early adapters 13.5% want benefits : want new technology for the sake of the benefits

Early majority 34% bandwagon : adapt to new technology when there’s evidence it’s good

Late majority 34% peer pressured : don’t like changing but will change when it’s necessary

Laggards 16% wusses : only adapt when they’re certain it won’t fail or they’re forced to

*What is meant by technology transfer?*

Transfer technology to other people, make it accessible to other users who can then further develop it

*State any two major factors that a software engineering company should consider when deciding whether or not to adopt a new technology.*

Cost, how much it’s been tested, time to adopt, is it backwards compatible with previous versions, testability(aka can you test it and then if you dont like it switch back or are you stuck with it), legacy systems supportable etc? (BS answer)

**Professional Qualifications:**

*Related to the professional practice of software engineering, what is the difference between licensing and certification?*

License is something you must get to practice, i.e. doctor or lawyer. Cert is optional and shows you’re proficient in something, as Sable puts it looks good on resume.

*What is legacy code? Why does such code often exist in a system?*

	Old crappy code left over because everyone was too lazy to update it. 

*When is the software life cycle complete?*

End of maintenance--when you no longer support the system

*Of the various stages that comprise the software life cycle, which stage often requires the most time and effort by software organizations?*

Usually maintenance 

MISC QUESTIONS

*Name any two ways that the field of software engineering has changed significantly in the past 15 or so years.*

Object oriented technology? Agile/extreme programming	

*Related to the evaluation of software engineering processes, what is a post-mortem analysis?*

Assessment of all aspects of project after delivery.

1. project survey - ask devs about tools used

2. collecting objective info 

3. debriefing meeting

4. project history day

5. publish the results

*Related to decision making, what is the purpose of the Delphi technique?*

	Have different groups of "experts," first group anonymously reviews a software, next group sees previous reviews and adds their reviews and what they’d change from the first guys’, keep doing that and eventually get “ideal” review

*What is the difference between black-box reuse and clear-box reuse?*

* black-box reuse (ninja the entire thing- reuse code exactly as-is)

* white-box reuse (use a little bit of code- see that it’s similar to what you need and modify a bit)

*Three of Wasserman's eight fundamental notions of software engineering are: analysis and design methods and notation; software process; reuse. For each of these, specify something we have covered in class that relates to this.*

Wasserman’s Fundamental Notions For Effective Software Engineering

* Abstraction

* Analysis and Design Methods And Notations

* UI Prototyping

* System architecture

* Software process

* Reuse

* Measurement

* Tools and Integration

What sort of procedures does a software organization need to employ in order to successfully reuse its software components in future products?

Information retrieval??? ← get all the available information about the components?

*What is a software reliability model?*

Models the probability of error (eg. u-plot)

*What sort of evidence exists in the literature suggesting that decision makers in the workplace do not always make rational decisions?*

People generally decide the first idea that seems reasonable (not necessarily the best) ← ??????

*Which organizations have joined together to create a software engineering code of ethics?*

ACM & IEEE

Actual Quiz 2015 Answers:

1. Mostly large projects for a single company

2. Some developers come together to create software, opensource and get donations ← not paid. Can be any level of open source.1. Large proj for company2. Large proj for mass use3. Small to med proj for small business

3. Corrective: fixing broken things, squashing bugs foundAdaptive: change program to be useable currently, adapt to new standards, i.e new input, new osPerfective: make code betterPreventative: change to prevent future faults 

4. Low morale - people don’t want to upkeep + maintainers are thought of as lower :(Increasing complexity - maintainers have to understand and keep updating Pressure to fix quickly - may make easy fixes, not necessarily good ones since it can make more bugs Increasing complexity and Pressure to fix quickly fall under maintainer’s hard jobsDowntime vs Uptime: Don’t want to take system offline but need to balance maintenance timeHard to test: Since released, hard to test new changes(Instructor comment: Only needed one)

5. Skipped

6. Black box: take code reuse no changes i.e. math libraryWhite box - look at code and try to adapt and use parts you need

7. CMM - surveys people can lie does not evaluate developer’s quality doesn’t look at how good people are

8. Code reuse is good generally (Instructor notes: mixed results, reusing heavily modified code can results in faults) military study on fin software saw that there was a lot of redundancy and led to 60% reuse of code increased productivity) Points off: -1

9. In retrospect, they did a good post-mortem analysis. Devs were honest, found problem

10. Skip

11. License is need to practice like docs and lawyers. Cert is optional shows proficiency and looks good on resume

12. ACM and IEEE

