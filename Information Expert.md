The Information expert assigns the responsibility of X if X has information to fulfil that responsibility, its useful to assist in understandability, maintainability and extendibility.
Useful where a design model may have many classes with many responsibilities, given object X, allows us to understand which responsibilities can be assigned to X. Useful to address where IE can go through the design model and then if not present, in the domain model.
It is important to understand that you don't always need IE, usually resulting in problems with  dependencies.
For example, storing sale transaction in DB.
By expert, Sale should be responsible, but DB handling (SQL) is not related to logic of problem, DB logic class increases representational gap, and a DB logic in every class is required, with greater dependence, need more responsibility and therefore poor design.
#### Examples:
![[Pasted image 20241024103731.png]]
![[Pasted image 20241024103748.png]]![[Pasted image 20241024104127.png]]