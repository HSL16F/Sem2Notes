Aims to create [[Pure Fabrication]] object called factory which handles creation. Comes as a result of responsibility of creating objects when special considerations such as complex creating logic.
A Concrete factory is a simplified version of the GoF Abstract Factory Pattern.
Separates responsibility of complex creation into cohesive helper objects, hides complex logic, better memory management and performance.
Factory pattern does have issue of how to crate factory and access it, often only one instance of factory is needed, good practice to use singleton pattern, provide single access point through global visibility.
#### Examples
![[Pasted image 20241024220532.png]]
