# Clean Code Book 
- This book is divided into three sections. 
- section 1 is about more principles, conception and techniques. 
- section 2 is about cases that are needed to refactor and debugging. 
- section 2 is about us because we take action to correct bad codes. 

 

## 1 - Clean Code. 
Bad code becomes when you are in a rush to production. Adding more features to the app before make good the previous ones.
Owning a mess can decrease the productivity over the course of time. Also Code base will be redesigned. It requires more developers to engage. 
Developers are responsible for good code. Not a schedule, marketing types, users and managers. These will not be execuses for their code. Do not blame others. 
Make the deadline, you should think about to make code as clean as possible at all times.
- clean code is pleasing to read.
- clean code is handling the errors. 
- clean code contains only nessasary. 
- clean code is like abstraction. 
- clean code can by changed by other people rather than only the author. 
- clean code has tests.
- clean code shoulde be smaller.
- clean code is cared by coder. 
- clean code minimize number of entities. 
- clean code contains no duplication. 
- clean code is built on simple abstraction early than later. 
- clean code does only one thing. Do not take all the responsiblity. 

## 2 - Meaningful Names.
In my opinion, it is best to use AI agent to name variable, functions, classes and everything. Because they are better than humans at it. 
Giving a good, expressive name avoid writing complex comments. 

- Use Intention-Revealing Names
- Avoid Disinformation
- Make Meaningful Distinctions
- Use Pronounceable Names
- Use Searchable Names
- Avoid Encodings
- Member Prefixes
- Avoid Mental Mapping
- class name should be noun, methods shoulde be verb. 
- Pick One Word per Concept.
- Don’t Pun.
- Use Solution Domain Names.
- Use Problem Domain Names.
- Don’t Add Gratuitous Context.

## 3 - Functions 
Funstions are core of every programs. When you make your function good, your program will be good. 
First when you name your function, it should do exactly that you name it. 
- small 

Small functions always are better, because they are easy to look up, examine and even debugging. 

- Do One Thing

One function must do only one thing at time. It should not fetch, manipulate and save at time. 

- One Level of Abstraction per Function.
- Reading Code from Top to Bottom: The Stepdown Rule.
- Switch Statements.
- Use Descriptive Names.
- Function Arguments.
- Common Monadic Forms.
- Flag Arguments.
- Dyadic Functions. 
- Triads.
- Argument Objects.
- Argument Lists. 
- Verbs and Keywords. 
- Have No Side Effects. 
- Output Arguments. 
- Command Query Separation.
- Prefer Exceptions to Returning Error Codes.
- Error Handling Is One Thing. 
- Structured Programming.

## 4 - Comments. 
Comments actually are for bad code. When you had written code and realized a mess. You would use comment, 
However the brilliant code is with a fewer comment. It is best to clean up your code rather than using comments.
Keep in mind, however, that the only truly good comment is the
comment you found a way not to write.

- Comments Do Not Make Up for Bad Code. 
- Explanation of Intent. 
- Clarification. 
- Warning of Consequences.
- TODO Comments.
- Mumbling. bad comments
- Redundant Comments. bad comments. 
- Misleading Comments. bad.
- Mandated Comments. bad. 
- Commented-Out Code. bad. 

## 5 - Formatting. 
When it comes to formatting in a team. All members have to discuss to use what formatting style and they must imply this formatting rule. 

- Vertical Formatting. 
- The Newspaper Metaphor. 
- Vertical Openness Between Concepts. 
- Vertical Density. 
 
## 6 - Objects and Data Structures. 
- Hiding implementation is about abstractions!
- Objects hidetheir data behind abstractions and expose functions that operate on that data.
- Data structure expose their data and have no meaningful functions

 Procedural code makes it hard to add new data structures because all the functions mustchange. OO code makes it hard to add new functions because all the classes must change.
 So, the things that are hard for OO are easy for procedures, and the things that are
hard for procedures are easy for OO!

- The Law of Demeter.

Objects expose behavior and hide data. This makes it easy to add new kinds of objects
without changing existing behaviors. It also makes it hard to add new behaviors to existing
objects. Data structures expose data and have no significant behavior. This makes it easy to
add new behaviors to existing data structures but makes it hard to add new data structures
to existing functions.
In any given system we will sometimes want the flexibility to add new data types, and
so we prefer objects for that part of the system. Other times we will want the flexibility to
add new behaviors, and so in that part of the system we prefer data types and procedures.
Good software developers understand these issues without prejudice and choose the
approach that is best for the job at hand.

##  7 - Error Handling. 
In short, things can go wrong, and when they do, we as programmers are responsible for making sure that our code 
does what it needs to do.

- Use Exceptions Rather Than Return Codes.
- Write Your Try-Catch-Finally Statement First.
- Use Unchecked Exceptions.
- Provide Context with Exceptions. 
- Define Exception Classes in Terms of a Caller’s Needs. 
- Define the Normal Flow.
- Don’t Return Null. 
- Don’t Pass Null. 

## 8 - Boundaries.
- Using Third-Party Code.
- Using Code That Does Not Yet Exist.
When we want to use third party library in our project. We should write test, wait.. TEST!. You could say Testing 
3 rd part library is not our job, yeah you are right. But It helps us to learn the 3 rd party library and it costs 
nothing to us. So, it is called Learning Test. 

 Clean Boundaries.
 
Interesting things happen at boundaries. Change is one of those things. Good software
designs accommodate change without huge investments and rework. When we use code
that is out of our control, special care must be taken to protect our investment and make
sure future change is not too costly.
Code at the boundaries needs clear separation and tests that define expectations. We
should avoid letting too much of our code know about the third-party particulars. It’s better
to depend on something you control than on something you don’t control, lest it end up
controlling you.
We manage third-party boundaries by having very few places in the code that refer to
them. We may wrap them as we did with Map, or we may use an ADAPTER to convert from
our perfect interface to the provided interface. Either way our code speaks to us better,
promotes internally consistent usage across the boundary, and has fewer maintenance
points when the third-party code changes.

## 9 - Unit tests. 

- The Three Laws of TDD. 

1. You may not write production code until you have written a failing unit test.

2. You may not write more of a unit test than is sufficient to fail, and not com-
piling is failing.


3. You may not write more production code than is sufficient to pass the cur-
rently failing test.

- Tests Enable the -ilities. 
- Clean Tests. 
- Domain-Specific Testing Language. 
- One Assert per Test. 
- Single Concept per Test. 
