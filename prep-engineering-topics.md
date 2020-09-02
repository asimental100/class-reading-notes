Quantity trumps Quality: When it comes to software, the same rule applies. If you aren't building, you aren't learning. Rather than agonizing over whether you're building the right thing, just build it. And if that one doesn't work, keep building until you get one that does.

Clean Code: Chapter 1: Messy code leads to slowdowns and it is better to plan ahead and write slowly in order to ensure that you're code is clean. "True professionals know that the second part of the conundrum is wrong. You will not make the deadline by making the mess. Indeed, the mess will slow you down instantly, and will force you to miss the deadline. The only way to make the deadline—the only way to go fast—is to keep the code as clean as possible at all times." & "It’s not enough to write the code well. The code has to be kept clean over time. We’ve all seen code rot and degrade as time passes. So we must take an active role in preventing this degradation."

TDD Red, Green, Refactor: The red, green, refactor approach helps developers compartmentalize their focus into three phases:
  1. Red — think about what you want to develop and write a test that informs the implementation of a feature. The test will only pass when the its expectations are met.
  2. Green — think about how to make your tests pass. The goal is to find a solution, without worrying about optimizing your implementation.
  3. Refactor — think about how to improve your existing implementation.
  
Cycles of TDD:
  Second-by-Second nano-cycle - The Three Laws of TDD:
    1. You must write a failing test before you write any production code.
    2. You must not write more of a test than is sufficient to fail, or fail to compile.
    3. You must not write more production code than is sufficient to make the currently failing test pass.
  Minute-by-Minute - micro-cycle: Red-Green-Refactor:
    1. Create a unit tests that fails
    2. Write production code that makes that test pass.
    3. Clean up the mess you just made.
