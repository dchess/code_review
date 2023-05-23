# Code Review Checklist
## Prerequisites before review
- A README
- Functional
- Checked into source control

## General
- Does it work? Does it meet functional requirements?
- Is the commit too large to review at once? (LOC > 500/hour)
- Does it have good commit messages?
- Is your commit up to date with master? (can it be merged without conflicts?)
- Does your new code add dependencies? Are they justified?
- Is there any documentation? (not just comments)
- Any redundant or duplicate code?
- Is it modular?
- Can any globals be replaced?
- Do loops have termination conditions?
- Does it have any obvious security holes?

## Basic formatting
- Naming conventions (Pascal, Camel, Snake case)
- Line length (80 chars)
- Commented code removed
- White space and code blocks
- Has a linter been used or code conventions followed?

## Testing
- Does it need tests?
- Does it have tests?
- Does it pass tests?
- Are the right things tested?
- Are edge cases tested?
- How can you break it?

## Architecture
- Separation of concerns (Layers: Business, Presentation, Data)
- Split by file type
- Design patterns

## Best Practices
- No hard coding (use constants/config vars)
- Proper use of data types
- Comments for why not what (also use To Do)
- Proper use of libraries and frameworks 
- Meaningful variable/function names
- Small functions
- Don’t return null
- DRY (Don’t repeat yourself)
- YAGNI (You aren’t gonna need it)
- Defensive inputs

## Non-functional Requirements
- **Readability** -- Self explanatory and easy to update
- **Testability** -- Can be mocked and tested easily
- **Debuggability** -- Logging, exceptions, and flow control
- **Configurability** -- Config vars modifiable without modifying code
- **Scalability** -- Time to task, concurrency limits, impacts on scale?

## Object Oriented Principles ([SOLID](https://www.freecodecamp.org/news/solid-principles-explained-in-plain-english/))
- Single Responsibility Principle
- Open/Closed Principle
- Liskov Substitution Principle
- Interface Segregation Principle
- Dependency Inversion Principle

