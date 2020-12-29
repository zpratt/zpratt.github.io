# Episode 1: Why is TDD so hard?

## TDD takes time to learn
* Start simple and make a goal: What outcome do you want to achieve by learning TDD?
* Demystify: Unit tests are just programs that call the public API of your production code and assert expected outcomes
* Experiment: Write a test that will filter a list of items
* Focus on Arrange, Act, Assert

## TDD doesn’t have a single definition, but is surrounded by dogma
* Test Driven Development, Test Driven Design, Emergent Design
* Ask yourself: do you value feedback loops? How often do you want feedback on how your code works, given a set of inputs and expected output?
* How does TDD relate to waterfall?
  * Waterfall SDLC: Design -> Build -> Test -> Run
    
## Organizations do not always create environments where TDD can flourish
* What is your organization’s culture?
  * Feature factories: Guessing at what the customer wants
  * Death marches: Deadline Driven Development
  * Are you on a team or are you a team of 1?
  * Do you have products or projects?
* Unclear definition of the What
* Can you and/or your team break down work?
* Do you have user stories, tasks, or something else? How do you know What you are supposed to build?

## TDD requires you to turn assumptions into assertions of fact
* An understanding of the What is needed
* What behavior am I focused on?
* Is that behavior driven by the user or the system?