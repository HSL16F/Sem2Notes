Creator exists to solve problem of who is responsible for creating new instance of class A. Good responsibility of assignment with creator allows for low coupling.
Creator exists to assign class B the responsibility to create more instances of Class A given one or more conditions are true (Generally more the better)
- B contains or compositely aggregates A
- B records A
- B closely uses A
- B has initialising data for A
Contradictions to keep in mind is that creating objects can lead to greater complexity
The creator can be delegates with helper classes such as [[Concrete Factory]] or [[Abstract Factory]]
### Example and use cases:
![[Pasted image 20241024103307.png]]