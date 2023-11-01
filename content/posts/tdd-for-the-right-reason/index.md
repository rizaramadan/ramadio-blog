+++
title = 'Doing TDD for the Right Reason: Its Okay to Do It Wrong'
date = 2023-10-11T23:01:42+07:00
draft = false
+++
In short, use TDD for the survival of the business. 

## Inflation
We inhabit a world where inflation is inescapable. It gradually erodes our assets, steadily diminishing their value until little or nothing remains. Businesses, too, are not immune to the impacts of inflation, making growth the sole sustainable strategy for survival. 

## How To Grow Business
Software is only valuable if it has features that customers use, and these features assist them in some way. By "features," I also mean content, non-functional aspects, and so on.

Thus, we can deduce that in the context of a software business, growing the business equates to expanding features. One of the most evident ways to increase features sustainably is by ensuring stability and a gradual reduction in the marginal cost of features. The marginal cost of features refers to the expense involved in developing the next feature.

## How To Reduce Marginal Cost of Features
Let me provide an example. Let's say we're developing a web app, and the first module we develop is user registration. Next, we want to develop a login module. It's almost certainly simpler to just add the login module to the previously developed user registration module. This is a no-brainer. But why, if the existing codebase has hundreds of modules, are we more inclined to separate the new module into a new repository?

The answer lies in the degree of modularity and abstraction of the existing codebase. A codebase with low modularity and poor abstraction will intimidate developers, making them more inclined to create a new codebase. In contrast, highly modular and well-abstracted software will be a pleasure to work with. More importantly, it's one of the surefire ways to reduce the marginal cost over time.

## How To Make Highly Modular & Well Abstracted Software
Some methods enable us to develop highly modular and well-abstracted software, but I would argue that these methods are quite hard to grasp. Is there another approach that's easier to understand to help us achieve this?

Fortunately, the answer is yes. While it may be challenging to execute TDD (Test-Driven Development), understanding its principles is not too difficult. Embracing TDD is a step towards creating highly modular and well-abstracted software.

# Conclusion
Inflation compels businesses to grow in order to survive. Growth becomes exponentially easier if generating value becomes easier over time (in the context of the software business, "value" means features). Making it easier to create more features over time can be achieved by developing highly modular and well-abstracted software. TDD is one of the most straightforward approaches that guide us toward creating highly modular and well-abstracted software. In short, use TDD for the survival of the business. 