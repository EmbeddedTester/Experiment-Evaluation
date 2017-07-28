# Traditional Setup vs. Pairing vs. Mobbing - Experiment Evaluation

## Aim 
We want to investigate the influence of the collaboration model on the work output of a team.

## Method

### Group Size
We had 11 attendees for the experiment. We randomly split the participants into two groups of 5 and 6 people.

### General

We used a web application with several bugs in it. For each setup the teams got a different version of the same application containing a similar amount and similar complexity of bugs. The two teams worked in the same setup but on different versions of the application at the same time.


|Setup|Group A|Group B|
|------|-------|-------|
|Traditional| Web App Version A | Web App Version B |
|Pairing|Web App Version B | Web App Version C|
|Mobbing|Web App Version C|Web App Version A|

For each session we had preparation and explanation time of about 15 minutes. The team had one hour per session to work on the application. 

The teams were supposed to test the application, find bugs in it and fix the bugs. When the team felt like they found all bugs in the application, they could implement new features. The team was asked to find a way to communicate about found bugs, to organise the work distribution and to have all the code changes on one machine at the end of the session.

After each round the team was asked to fill out a survey containing the following questions:

- How many bugs did you find? 
- How many bugs did you fix?
- How many user stories did you implement?
- How much fun did you have? Scale 1 (No fun at all) -5 (Lots)
- How would you rate the quality of the work you did? Scale 1 (Poor) -5 (Excellent)

We also had a quick standup with both teams after the one-hour session where we would ask some additional questions like:

- Which tasks are left to do, e.g. retesting bug fixes, merging the code?
- How much do you know about what the other team members worked on?
- How much do you know about how the other team members fixed a bug?

### Traditional Setup
We started with a traditional team setup. The team members were asked to act in different roles, 2 testers and 3 or 4 developers. The testers started exploring the application and notified the developers about bugs via a bug tracking system or in one of the groups by raising their hands and showing the developer the bug. The developers started by getting familiar with the application until there was a bug they could work on. The developers worked on fixing the bug and notified the testers about fixed bugs.

### Pairing
Instead of having fixed roles, the team was working in pairs where every pair performed developing and testing activities. The pairs started investigating the new version of the application and used a flipchart to inform the other pairs about bugs found, work assignments and bugs fixed.

### Mobbing
In this team setup the whole team worked on one computer using a drive/navigator pattern where the team rotated the roles after 4 minutes in the beginning. After having one team member in every role once, it was open to the team to change how they work.
 
The teams used a flipchart to write down bugs they found while they were not driver or navigator or things they wanted to come back to at a later point.

## Variables 
### Dependent variables
- Number of bugs found (counted by the team)
- Number of bugs fixed (counted by the team)
- Number of implemented user stories (counted by the team)
- Fun (rated by the team)
- Quality of the work (rated by the team)

### Independent variable

Collaboration model:
- working alone on a task
- Pairing on a task
- Working as a group on a task

### Fixed variables
- The same team
- The same application (comparable versions of the application in regards to the number and the complexity of the bugs)

## Prediction
We expected:

 1. a similar amount of bugs to be found and fixed in both traditional and pairing
 2. less bugs to be found and fixed in mobbing
 3. pairing would be seen as more fun
 4. mobbing and pairing to be seen a higher yielding higher quality  

## Results 
### Group A

|#Bugs found|#Bugs fixed|#User Stories|Fun|Quality|
|------|-------|-------|-------|-------|
|Traditional|9|5|0|4|4|
|Pairing|9|9|1|5|5|
|Mobbing|9|8|0|4|4|

### Group B
|#Bugs found|#Bugs fixed|#User Stories|#Fun|#Quality|
|------|-------|-------|-------|-------|
|Traditional|6|4|1|4|4|
|Pairing|10|8|0|4|4|
|Mobbing|8|8|0|4|4|

## Conclusion 
Group A showed a consistency over the three sessions in finding bugs and group B showed a slight improvement when working in pairs. The trend for fixing bugs was similar across both teams, showing a distinct improvement in pairing. 

It should also be noted that while working on the embedded scenario, two of the “developers” in team A gravitated towards pairing. This is an indicator that some people will naturally pair when confronted with an unknown system. 

From the results here, mobbing seems to have some merit. Most managers might be afraid that productivity would drop dramatically having all team members working on the same problem. However, the results here suggest that this may not be the case. On top of this, at the end of the mobbing session all team members knew about the bugs found, how they were fixed, the bug fixes were tested again and the code was merged on one machine.

Our expectation that mobbing and pairing would be seen to yield higher “quality” was not reflected in the results.  The same can be said for thinking that pairing would be seen as more “fun”. 

From the given results, we would conclude that it is still inconclusive which method is indeed the best. Given the similar stats on productivity, we would nevertheless encourage teams to experiment with pairing and mobbing. 

## Evaluation 

The experiment lacks enough controls to be fully considered scientific. Given that this experiment was carried out at a conference, we wanted to give the participants a similar experience. 

Furthermore, due to this setup, the members may have been less inclined to say that a particular session was “not fun” (i.e. < 3) or that they produced “poor quality”. These are things that are very hard to quantify, especially given no guidelines for what constitutes “quality” or “fun”. These characteristics will only be truly seen over a significant amount of time; for example by tracking bugs introduced or by team attrition rate.

Some of the potential benefits of pairing/mobbing will only show after a while, e.g. better overall understanding of the system, higher quality of the product.

Despite all this, we would still encourage teams to try these methods. Here are a number of suggestions on how one could improve on our experiment.

- A control group who do the three sessions using only traditional
- Have a third group, and have each group work using a different method in parallel
- Quantify knowledge of the system as a whole within the team
-- How much of the system does each individual understand. 
-- By pairing information dissemination is part of the day to day process and doesn’t need to be incorporated in “knowledge transfer” sessions, which eat up a lot of time
- Quantify time saved on code reviewing
-- Especially in mobbing, code review is no longer required - everyone was there.

### Influencers:

The experiment might have been also influenced by the following:

- Teams learned about the application during the day. Although each version of the application was different, it might be that they were faster because of that.
- Group consisted mainly of testers, some with development experience
- Different versions of the application might not have exactly the same complexity in regards to finding and fixing bugs. We tried to mitigate by rotating the versions

## References

[Woody Zuill and Kevin Meadows: Mob Programming A Whole Team Approach] (https://leanpub.com/mobprogramming )

[Maaret Pyhäjärvi and Llewellyn Falco: Mob Programming Guidebook] (https://leanpub.com/mobprogrammingguidebook)

[Elisabeth Hocke: Our Team's First Mobbing Session](http://www.lisihocke.com/2017/05/thoughts-about-testing-in-a-mob.html)

[Llewellyn Falco: Strong-style pairing] (http://llewellynfalco.blogspot.de/2014/06/llewellyns-strong-style-pairing.html )




