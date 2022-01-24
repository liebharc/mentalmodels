# Mental models

Some notes about mental models. I want to visualize them to make transparent to others, why I take certain positions and to allow them to not only challenge what I say, but to also challenge my mental models directly.

## Cost of IT projects/features over time

Here is a rough sketch on how I perceive the cost of a typical IT project or new feature over time:
![Cost of TI projects](/img/CostOfAProjectOverTime.png)

1. Planning happens and the more concrete an idea gets, the more people get involved. Perhaps screen mocks are crated, some prototypes are done or project plans are created. So over the time the cost for a feature already increases, before the actual work is done.
2. The feature is worked on. Teams push the development forward.
3. The feature is officially released. But work is needed to respond to customer questions, fix defects and perform cleanup tasks.
4. The feature enters a maintenance phase. Occasionally support questions need to be answers, defects are fixed or security patches installed.

In this model I find the maintenance part very interesting. Because for the company usually the feature is done and no one thinks of it anymore. But it continues to create work. And this is true for all your features. So as more and more features get added, the maintenance tasks sum up drastically. It the end it might consume large parts of your development capacity and decrease the performance of your company. Thus care needs to be taken to keep the maintenance part small.

# Technical debt

A lot of code I'm working with in companies is several years old. People might be surprised and think that software changes very quickly - and it does. Both statements are true, a lot of code is very old why it constantly receives modifications and the code and technology around it changes. That means
that developers need to write code which works together with concepts which don't exist yet. Usually a developer rather quickly writes code which does the job, and then spends time to make it well enough to be: Flexible, Testable, Reusable, and Documented.

If there is an important release, then the question arises if the release can be rushed out by skipping steps. The answer is: Yes, and it might be a tool which one wants to keep in mind. But there is a big "BUT". With that decision you will hit issues in the future. This goes so far, that I've seen companies which are basically unable to move anymore due to technical debt (in the words of "Cost of IT projects/features over time": Your maintenance cost went far too high over time). The concept of technical debt expresses this as well: Every time you rush a release, you build up debt which you have to pay back in future. As with all debt, it's cheaper to pay it back sooner than later. That's because over time workarounds get added to deal with the issues which a rushed release left behind. So ofter time you don't just have to cleanup your rushed decisions, but also all workarounds which have been created meanwhile.

![Technical Debt](/img/TechnicalDebt.png)
