# refactoring-2nd-edition
My notes for Refactoring 2nd edition by Martin Fowler

## Chapter 01
- When you have to add a feature to a program but the code is not structured in a convenient way, first refactor the program to make it easy to add the feature, then add the feature.
- Features requests will change again within six months.

- **Refactor Steps #1: Create Tests** 
    - Ensure to have solid suite of tests for that section of code. 
    - The tests are essential to avoid introducing bugs. As humans, we can make mistakes.
    - These tests must be self-checking.

- **Refactoring Steps #2: Decompose Large Functions**
    - In decomposing large functions, the first step is to eyeball the code and look for groupings or chunks. These can be conditionals (switch or an if-else block), commented code, or even line spacing.
    - Extract the chunk of code into a separate function and name accordingly. This method is also knows as **Extract Fuction**.
    - Refactor code in smalls steps so it is easy to find any bugs introduced.
    
- **Refactoring Steps #3: Refactor, Test and Commit** 
    - Test code after small changes.
    - **TIP: Use git to commit every successful refactoring**
    - This allows us to easily get back to a working state should we mess up later.
    - Squash changes into significant commits before pushing to remote.

- **TIP: You can use the name "result" for the return value in a function.**

- **NOTE:** What about performance?
    - Performance is important but refactoring always comes first.
    - Refactored code makes performance tuning better and more effective.

- **Recatoring Steps #4: Replace Conditionals with Polymorphism**
    - Large switch and if blocks are glaring issues and must be transferred to separate classes.
    - This ensures readability and making into code smaller bits.

- **Rectoring methods used in Chapter 01:**
    - Extract Function
    - Inline Variable
    - Move Function
    - Replace Conditional with Polymorphism
    - Split Phase

- **Final Thoughts:**
    - The true test of good code is how easy it is to change it.
    - Code should be obvious: When someone needs to make a change, they should be able to find the code to be changed easily and to make the change quickly without introducing any errors.